---
title: Enhet i vänte läge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679993"
---
# <a name="device-in-pending-state"></a>Enhet i vänte läge

**Förutsättningar**

1. Om du ställer in enhets registreringarna första gången bör du kontrol lera att du har granskat [introduktionen till enhets hantering i Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som hjälper dig att hämta enheter under kontrollen av Azure AD.
2. Om du registrerar enheter till Azure AD direkt och registrerar dem i Intune måste du se till att du har [konfigurerat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) och har [licensierat](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) först.
3. Se till att du har behörighet att utföra åtgärder i Azure AD och lokala annonser. Endast globala administratörer i Azure AD kan hantera inställningar för enhets registreringar. Om du konfigurerar automatiska registreringar i lokala Active Directory måste du dessutom vara administratör för Active Directory och AD FS (om tillämpligt).

För registrerings processen för Azure AD Join krävs enheter för företags nätverk. Den fungerar också via VPN, men det finns vissa villkor för detta. Vi har hört att kunder behöver hjälp med att felsöka registrerings processen för Azure AD Join under andra arbets förhållanden.

**Molnbaserad miljö för moln (använder Azure AD-hash för lösen ord eller direktautentisering)**

Detta registrerings flöde kallas också "Sync Join".

Här är en uppdelning av vad som händer under registrerings processen:

1. Windows 10 upptäcker tjänst anslutnings punktens post (SCP) när användaren loggar in på enheten.

    1. Enheten försöker först hämta klient information från klient-SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Mer information finns i [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Om det Miss lyckas kommunicerar enheten med lokal Active Directory för att få information om klient organisationen från SCP. Om du vill verifiera SCP läser du det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Vi rekommenderar att du aktiverar SCP i Active Directory och bara använder klientens SCP för initial verifiering.

2. Windows 10 försöker kommunicera med Azure AD under system kontexten för att autentisera sig mot Azure AD.

    Du kan kontrol lera om enheten kan komma åt Microsoft-resurser under system kontot med hjälp av [test enhetens registrerings skript för registrering](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 skapar ett egensignerat certifikat och lagrar det under datorobjektet i lokala Active Directory. Detta kräver att en domänkontrollant används för att kontrol raden.

4. Enhets objekt med certifikat synkroniseras till Azure AD via Azure AD Connect. Synkroniseringen är 30 minuter som standard, men det beror på konfigurationen av Azure AD Connect. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. I det här steget ska du kunna se ämnes enheten i "**förestående**" tillstånd under enhets bladet i Azure Portal.

6. Vid nästa användar inloggning till Windows 10 kommer registreringen att genomföras.

    > [!NOTE]
    > Om du använder VPN och utloggning/inloggning säger upp domän anslutningen kan du utlösa registreringen manuellt. Så här gör du:
    >
    > Skicka ett `dsregcmd /join` lokalt i administratörs meddelande eller fjärrans luta via PsExec till datorn.
    >
    > Till exempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Vanliga frågor och [svar](https://docs.microsoft.com/azure/active-directory/devices/faq)om Azure Active Directory-registrering.
