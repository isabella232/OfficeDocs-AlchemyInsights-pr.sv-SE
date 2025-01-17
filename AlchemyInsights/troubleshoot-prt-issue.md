---
title: Felsöka PRT-problem
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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330977"
---
# <a name="troubleshoot-prt-issue"></a>Felsöka PRT-problem

För att en enhet ska kunna autentiseras måste den vara fullständigt registrerad och i gott skick och kunna skaffa en primär uppdateringstoken (PRT).

Registreringsprocessen för hybrid-Azure AD-anslutning kräver att enheter finns på ett företagsnätverk. Det fungerar även via VPN, men det finns vissa varningar. Vi har hört kunder som behöver hjälp med att felsöka registreringsprocessen för hybrid-Azure AD-anslutning under fjärrarbete. Så här går det till under registreringsprocessen:

**Molnautentiseringsmiljö (med hjälp av azure AD-synkronisering av lösenordshashar eller direktautentisering)**

Det här registreringsflödet kallas även "Synkroniseringskoppling".

1. Windows 10 identifierar en SCP-post när användaren loggar in på enheten.
    1. Enheten försöker först hämta information om klientorganisationen från klientsidans SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Om det inte fungerar kommunicerar enheten med lokal Active Directory (AD) för att få information om klientorganisationen från Service Connection Point (SCP). Information om hur du verifierar SCP finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

**Obs!** Vi rekommenderar att du aktiverar SCP i AD och bara använder SCP på klientsidan för första valideringen.

2. Windows 10 försöker kommunicera med Azure AD under systemkontexten för att autentisera sig mot Azure AD. Du kan kontrollera om enheten kan komma åt Microsoft-resurser under systemkontot med hjälp av skriptet Test Device Registration Connectivity.

3. Windows 10 genererar ett själv signerat certifikat och lagrar det under datorobjektet i en lokal AD. Det här kräver synhåll för domänkontrollanten.

4. Ett enhetsobjekt som har ett certifikat synkroniseras till Azure AD via Azure AD Anslut. Som standard är synkroniseringscykeln var 30:e minut, men det beror på konfigurationen av Azure AD Anslut. Mer information finns i det här [dokumentet.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. I det här läget bör du kunna se ämnesenheten i läget "Väntande" under Enhetsblad i Azure Portal.

6. Vid nästa inloggning till Windows 10 slutföras registreringen. 

**Obs!** Om du använder VPN och en logoff-login-process avslutar domänanslutningen kan du utlösa registreringen manuellt:
 1. Skapa ett dsregcmd /join lokalt i administratörsfrågan eller via PSExec på datorn. Till exempel, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Mer information om hybridkopplingsproblem finns i [Felsöka problem med enheter.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
