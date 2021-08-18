---
title: Enhet i väntande tillstånd
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
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330390"
---
# <a name="device-in-pending-state"></a>Enhet i väntande tillstånd

**Krav:**

1. Om du inställningar enhetsregistreringar för första gången bör du kontrollera att du har granskat Introduktion till enhetshantering i [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som vägleder dig om hur du får enheter under kontroll av Azure AD.
2. Om du registrerar enheter i Azure AD direkt och registrerar dem i Intune måste du se till [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) att du har konfigurerat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) och har licensieringen först.
3. Se till att du har behörighet att utföra åtgärder i Azure AD och lokalt AD. Endast en global administratör i Azure AD kan hantera inställningar för enhetsregistreringar. Om du konfigurerar automatiska registreringar i din lokala Active Directory måste du dessutom vara administratör för Active Directory och AD FS (om tillämpligt).

Registreringsprocessen för hybrid-Azure AD-anslutning kräver att enheter finns på företagets nätverk. Det fungerar även via VPN, men det finns vissa varningar. Vi har lyssnat på kunder som behöver hjälp med att felsöka registreringsprocessen för hybrid-Azure AD-anslutning under fjärrarbete.

**Molnautentiseringsmiljö (med hjälp av azure AD-synkronisering av lösenordshashar eller direktautentisering)**

Det här registreringsflödet kallas även "Synkroniseringskoppling".

Här är en sammanfattning av vad som händer under registreringsprocessen:

1. Windows 10 identifierar SCP-posten (Service Connection Point) när användaren loggar in på enheten.

    1. Enheten försöker först hämta information om klientorganisationen från klientsidans SCP i registret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Mer information finns i [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Om det inte fungerar kommunicerar enheten med lokal Active Directory för att få information om klientorganisationen från SCP. Information om hur du verifierar SCP finns i [det här dokumentet.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Obs!** Vi rekommenderar att du aktiverar SCP i Active Directory och bara använda SCP på klientsidan för första valideringen.

2. Windows 10 försöker kommunicera med Azure AD under systemkontexten för att autentisera sig mot Azure AD.

    Du kan kontrollera om enheten kan komma åt Microsoft-resurser under systemkontot med hjälp av [skriptet Test Device Registration Connectivity.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 genererar själv signerade certifikat och lagrar det under datorobjektet i lokalt Active Directory. Det här kräver synhåll för domänkontrollanten.

4. Enhetsobjekt som har certifikat synkroniseras till Azure AD via Azure AD Anslut. Synkroniseringscykeln är var 30:e minut som standard, men det beror på konfigurationen av Azure AD Anslut. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. I det här läget bör du kunna se ämnesenheten i läget "**Väntande**" under Enhetsblad i Azure Portal.

6. Vid nästa inloggning till Windows 10 slutföras registreringen.

    **Obs!** Om du använder VPN och inloggning avbryts domänanslutningen kan du utlösa registreringen manuellt. Så här gör du det:
    
    Skapa ett `dsregcmd /join` lokalt administratörsuppfråga eller via PSExec på datorn.\
    Till exempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Vanliga problem med registrering av Azure Active Directory finns i Vanliga frågor [och svar om enheter.](https://docs.microsoft.com/azure/active-directory/devices/faq)
