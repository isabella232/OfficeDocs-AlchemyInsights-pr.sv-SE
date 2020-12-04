---
title: Felsöka problem med PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573902"
---
# <a name="troubleshoot-prt-issue"></a>Felsöka problem med PRT

För att alla enheter ska kunna bli autentiserade måste de vara fullständigt registrerade och i gott skick och kunna skaffa en primär uppdateringstoken (PRT).

För registrerings processen för Azure AD Join måste enheter finnas i ett företags nätverk. Den fungerar också via VPN, men det finns vissa villkor för detta. Vi har hört att kunder behöver hjälp med att felsöka registrerings processen för Azure AD Join under fjärran slut omständigheter. Här är en uppdelning av vad som händer under registrerings processen.

**Molnbaserad miljö för moln (använder Azure AD-hash för lösen ord eller direktautentisering)**

Detta registrerings flöde kallas också "Sync Join".

1. Windows 10 upptäcker en SCP-post när användaren loggar in på enheten.
    1. Enheten försöker först hämta klient information från klient-SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Om det Miss lyckas kommunicerar enheten med lokal Active Directory (AD) för att hämta klient information från tjänst anslutnings punkten (SCP). För att verifiera SCP, hänvisa till det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Vi rekommenderar att du aktiverar SCP i ANNONSen och bara använder klient platsens SCP för initial verifiering.

2. Windows 10 försöker kommunicera med Azure AD under system kontexten för att autentisera sig mot Azure AD. Du kan kontrol lera om enheten kan komma åt Microsoft-resurser under system kontot med hjälp av test enhetens registrerings skript för registrering.

3. Windows 10 skapar ett självsignerat certifikat och lagrar det under datorobjektet i den lokala ANNONSen. Detta kräver att en domänkontrollant används för att kontrol raden.

4. Ett enhets objekt som har ett certifikat synkroniseras till Azure AD via Azure AD Connect. Synkroniseringen är 30 minuter som standard, men det beror på konfigurationen av Azure AD Connect. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. I det här steget ska du kunna se ämnes enheten i "förestående" tillstånd under enhets bladet i Azure Portal.

6. Vid nästa användar inloggning till Windows 10 kommer registreringen att genomföras. 

> [!NOTE]
> Om du använder VPN och en utloggning-inloggning avslutar domän anslutningen kan du utlösa registrering manuellt:
 1. Skicka en dsregcmd/Join lokalt i administratörs tolken eller fjärrans luta via PSExec till datorn. Till exempel PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Mer information om hybrid kopplings problem finns i [Felsöka problem med enheter](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
