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
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="28b3e-102">Jag blockeras av villkorsstyrd åtkomst med domän ansluten enhet</span><span class="sxs-lookup"><span data-stu-id="28b3e-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="28b3e-103">**Rekommenderade verktyg**</span><span class="sxs-lookup"><span data-stu-id="28b3e-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="28b3e-104">[Felsökaren för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) verktyget som hjälper till att felsöka de vanligaste enhetsregistreringsproblemen.</span><span class="sxs-lookup"><span data-stu-id="28b3e-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="28b3e-105">[Testa skript för enhetsregistrering –](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Skriptet som hjälper till att säkerställa att en enhet kan komma åt slutpunkter för enhetsregistrering under systemkontot.</span><span class="sxs-lookup"><span data-stu-id="28b3e-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="28b3e-106">[Azure AD-enhetsrensningsskript](https://github.com/mzmaili/AzureADDeviceCleanup) – Skriptet som gör att du kan söka efter och hantera inaktuella enheter i din miljö.</span><span class="sxs-lookup"><span data-stu-id="28b3e-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="28b3e-107">Här är några vanliga orsaker till att villkorsstyrd åtkomst inte fungerar på en enhet som har anslutit till en domän (Hybrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="28b3e-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="28b3e-108">**Det finns ingen Azure AD PRT** på enheten – Du måste kontrollera att enheten har primär uppdateringstoken för Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="28b3e-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="28b3e-109">Mer information om PRT finns i det här [dokumentet.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="28b3e-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="28b3e-110">Du kan kontrollera om du har Azure AD PRT genom att köra kommandot på enheten och kontrollera om `dsregcmd/status` "AzureAdPrt" är lika med "JA".</span><span class="sxs-lookup"><span data-stu-id="28b3e-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="28b3e-111">Om "AzureAdPrt" är "NO" kontrollerar du följande:</span><span class="sxs-lookup"><span data-stu-id="28b3e-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="28b3e-112">Om du har en **federerad** miljö med AD FS och den inte kan nås från användarnas hemnätverk : I det här fallet ska du se till att dina slutpunkter för användarnamnsmix är tillgängliga från extranätet.</span><span class="sxs-lookup"><span data-stu-id="28b3e-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="28b3e-113">Om ditt AD FS ligger bakom en VPN ser du till att användarna ansluter till VPN och loggar in på enheten igen.</span><span class="sxs-lookup"><span data-stu-id="28b3e-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="28b3e-114">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="28b3e-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="28b3e-115">**Om enhetens TPM** är felaktig och därmed inte kan autentisera enheten: Kontrollera "tpm.msc" för att se om statusen för TPM är "Ready".</span><span class="sxs-lookup"><span data-stu-id="28b3e-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="28b3e-116">Om inte kör du `dsregcmd/leave` enheten och låter den åter gå med i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28b3e-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="28b3e-117">Försök sedan igen.</span><span class="sxs-lookup"><span data-stu-id="28b3e-117">Then, try again.</span></span> <span data-ttu-id="28b3e-118">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="28b3e-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="28b3e-119">**Du använder en tredjepartsidentitetsprovider som inte har stöd för WS-Trust protokoll.**</span><span class="sxs-lookup"><span data-stu-id="28b3e-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="28b3e-120">Enligt beskrivningen i våra dokument fungerar inte azure AD-anslutna hybridenheter i det här fallet.</span><span class="sxs-lookup"><span data-stu-id="28b3e-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="28b3e-121">Kontakta din identitetsleverantör för support.</span><span class="sxs-lookup"><span data-stu-id="28b3e-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="28b3e-122">Användare använder Webbläsaren Chrome utan **Windows 10-konton** eller Office-tillägget Chrome använder inte automatiskt prten på AAD-anslutna enheter eller **AAD-anslutna enheter:** Det leder till att det inte går att använda enhetsbaserade villkorsstyrda åtkomstprinciper, med felmeddelandet "Oregistrerad enhet".</span><span class="sxs-lookup"><span data-stu-id="28b3e-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="28b3e-123">Om du vill använda Chrome korrekt måste du installera "Windows 10-konton" eller "Office-tillägg till användarnas Chrome-webbläsare" via SCCM eller Intune.</span><span class="sxs-lookup"><span data-stu-id="28b3e-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="28b3e-124">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="28b3e-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="28b3e-125">Om det inte går att skicka tillägget via fjärrstyrd push-anslutning meddelar du användarna att manuellt installera något av ovanstående tillägg för åtkomst till program bakom enhetsbaserade villkorsstyrda åtkomst.</span><span class="sxs-lookup"><span data-stu-id="28b3e-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="28b3e-126">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="28b3e-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="28b3e-127">Enheten var korrekt hybridansluten i Azure AD men den togs bort av misstag eller inaktiverades, antingen på grund av synkroniseringsändringar i Azure AD Connect eller från **Azure-portalen:** Om det händer identifieras inte enhetsobjektet längre som en fullständigt ansluten enhet även om statusen "AzureAdJoined" och "PRT" visas som giltig på enheten.</span><span class="sxs-lookup"><span data-stu-id="28b3e-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="28b3e-128">Åtgärda problemet genom att köra på `dsregcmd/leave` de enheter som påverkas och låta dem återansluta till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28b3e-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="28b3e-129">Mer information finns i det här [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="28b3e-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="28b3e-130">Om dina enheter använder Windows 10, 1809-uppdatering med VPN/molnproxy och du får problem med "AzureAdPrt"-status eller appar med SSO-problem (Outlook ansluter inte till postlådan trots att du hade PRT) bör du kontrollera att du har den här uppdateringen [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller aprils kumulativa uppdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) för att förhindra PRT-fel på dessa datorer.</span><span class="sxs-lookup"><span data-stu-id="28b3e-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















