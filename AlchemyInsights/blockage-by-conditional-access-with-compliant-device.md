---
title: Jag blockeras av villkorsstyrd åtkomst med kompatibel enhet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037078"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Jag blockeras av villkorsstyrd åtkomst med kompatibel enhet

**Rekommenderade verktyg**

- [Felsökaren för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) ett omfattande verktyg som hjälper dig felsöka de vanligaste problemen med enhetsregistrering.
- [Testa skript för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Ett verktyg som används för att säkerställa att en enhet kan komma åt slutpunkter för enhetsregistrering under systemkontot.
- [Azure AD-enhetsrensningsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – ett verktyg som används för att söka efter och hantera inaktuella enheter i din miljö.

Här är några vanliga orsaker till att villkorsstyrd åtkomst inte fungerar  för en enhet som är kompatibel eller varför användarna eventuellt får Meddelandet du kan inte hämta därifrån vid en inloggningsförfrågan till en organisationsresurs.

1. **Enheten är inte i nödvändig enhet med en MDM:**

Verifiera att enheten är registrerad med en godkänd MDM-leverantör som Intune och *markerad som kompatibel.* Mer information om Intune finns i det här [dokumentet.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Mer information om enhetsefterlevnad och Intune finns i Använda efterlevnadsprincip för att ange regler för enheter [som du hanterar med Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Om du har problem med att registrera en enhet med Intune hittar du felsökningsinformation i [Felsöka enhetsregistrering i Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Om du vill ha mer Intune-support skapar du en supportbegäran. Det gör du genom att gå [till sidan Hjälp och support för Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Enheten är inte ansluten till organisationens nätverk:**

För åtkomst till organisationsresurser måste enheten vara ansluten till organisationens nätverk, antingen via direktanslutning eller via ett virtuellt privat nätverk (VPN), och även ansluten till lokalt eller Azure Active Directory. Information om hur du ansluter till en arbetsenhet i organisationens nätverk finns i [Ansluta din arbetsenhet till organisationens nätverk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Information om hur du registrerar en personlig/BYOD-enhet [finns i Registrera din personliga enhet i organisationens nätverk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- För att verifiera om enheten har anslutit till nätverket kan du följa stegen för registrerade enheter [här](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) eller arbetsenheter [här](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Följ riktlinjerna nedan för att begränsa problemet till organisationsnätverksanslutning:

    1. Logga in på Windows med ditt arbets- eller skolkonto, till exempel genom att alain@contoso.com.
    2. Anslut till din organisations nätverk via ett VPN eller DirectAccess.
    3. När du är ansluten trycker du på **Windows-tangenten + L för** att låsa enheten.
    4. Lås upp enheten med ditt arbets- eller skolkonto och försök sedan få åtkomst till appen eller tjänsten med problem igen.

Om du ser **felmeddelandet Du kan inte komma dit härifrån igen** är problemet sannolikt någon annanstans.

3. **Operativsystemet stöds inte:**

Kontrollera att du kör en version av operativsystemet som stöds, inklusive:

- **Windows-klient:** Windows 7 eller senare

- **Windows Server:** Windows Server 2008 R2 eller senare

- **macOS**: macOS X eller senare

- **Android och iOS:** Senaste versionen av mobila operativsystem för Android och iOS

4. **Webbläsare stöds inte:**

Du hittar webbläsare som stöds nedan. För Chrome-stöd med Windows 1703 eller senare versioner krävs ett tillägg för Windows 10-konton. För Edge 85+ måste användaren vara inloggad för att kunna överföra information om enhetsefterlevnad korrekt. Mer information finns i [här](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/ 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge:** Intune Managed Browser, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Mer information om **anvisningarna för hur du inte hittar meddelandet** och felsökningsstegen hittar du [här.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
