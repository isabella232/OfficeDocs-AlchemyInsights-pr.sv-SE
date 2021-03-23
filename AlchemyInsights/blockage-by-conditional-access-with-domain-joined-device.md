---
title: Jag blockeras av villkorsstyrd åtkomst med domän ansluten enhet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038104"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Jag blockeras av villkorsstyrd åtkomst med domän ansluten enhet

**Rekommenderade verktyg**

[Felsökaren för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) verktyget som hjälper till att felsöka de vanligaste enhetsregistreringsproblemen.

[Testa skript för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Skriptet som hjälper till att säkerställa att en enhet kan komma åt slutpunkter för enhetsregistrering under systemkontot.

[Azure AD-enhetsrensningsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – Skriptet som gör att du kan söka efter och hantera inaktuella enheter i din miljö.

Här är några vanliga orsaker till att villkorsstyrd åtkomst inte fungerar på en enhet som har anslutit till en domän (Hybrid Azure AD).

1. **Det finns ingen Azure AD PRT** på enheten – Du måste kontrollera att enheten har primär uppdateringstoken för Azure AD (PRT). Mer information om PRT finns i det här [dokumentet.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Du kan kontrollera om du har Azure AD PRT genom att köra kommandot på enheten och kontrollera om `dsregcmd/status` "AzureAdPrt" är lika med "JA".

Om "AzureAdPrt" är "NO" kontrollerar du följande:

- Om du har en **federerad** miljö med AD FS och den inte kan nås från användarnas hemnätverk : I det här fallet ska du se till att dina slutpunkter för användarnamnsmix är tillgängliga från extranätet. Om ditt AD FS ligger bakom en VPN ser du till att användarna ansluter till VPN och loggar in på enheten igen. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Om enhetens TPM** är felaktig och därmed inte kan autentisera enheten: Kontrollera "tpm.msc" för att se om statusen för TPM är "Ready". Om inte kör du `dsregcmd/leave` enheten och låter den åter gå med i Azure AD. Försök sedan igen. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Du använder en tredjepartsidentitetsprovider som inte har stöd för WS-Trust protokoll.** Enligt beskrivningen i våra dokument fungerar inte azure AD-anslutna hybridenheter i det här fallet. Kontakta din identitetsleverantör för support.

2. Användare använder Webbläsaren Chrome utan **Windows 10-konton** eller Office-tillägget Chrome använder inte automatiskt prten på AAD-anslutna enheter eller **AAD-anslutna enheter:** Det leder till att det inte går att använda enhetsbaserade villkorsstyrda åtkomstprinciper, med felmeddelandet "Oregistrerad enhet". Om du vill använda Chrome korrekt måste du installera "Windows 10-konton" eller "Office-tillägg till användarnas Chrome-webbläsare" via SCCM eller Intune. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Om det inte går att skicka tillägget via fjärrstyrd push-anslutning meddelar du användarna att manuellt installera något av ovanstående tillägg för åtkomst till program bakom enhetsbaserade villkorsstyrda åtkomst. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. Enheten var korrekt hybridansluten i Azure AD men den togs bort av misstag eller inaktiverades, antingen på grund av synkroniseringsändringar i Azure AD Connect eller från **Azure-portalen:** Om det händer identifieras inte enhetsobjektet längre som en fullständigt ansluten enhet även om statusen "AzureAdJoined" och "PRT" visas som giltig på enheten.

Åtgärda problemet genom att köra på `dsregcmd/leave` de enheter som påverkas och låta dem återansluta till Azure AD. Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Om dina enheter använder Windows 10, 1809-uppdatering med VPN/molnproxy och du får problem med "AzureAdPrt"-status eller appar med SSO-problem (Outlook ansluter inte till postlådan trots att du hade PRT) bör du kontrollera att du har den här uppdateringen [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller aprils kumulativa uppdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) för att förhindra PRT-fel på dessa datorer.

















