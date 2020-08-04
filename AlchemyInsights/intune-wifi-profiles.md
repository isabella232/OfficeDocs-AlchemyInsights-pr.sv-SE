---
title: Intune Wi-Fi-profiler
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555815"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="10641-102">Intune Wi-Fi-profiler</span><span class="sxs-lookup"><span data-stu-id="10641-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="10641-103">En lyckad implementering av Wi-Fi-anslutning för MDM-klienter beror på en korrekt distribuerad profil som återspeglar kraven för företagets Wi-Fi-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="10641-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="10641-104">Information om hur du granskar lämpliga inställningar för klientplattformarna som du undersöker finns i:</span><span class="sxs-lookup"><span data-stu-id="10641-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="10641-105">Lägga till Wi-Fi-inställningar för enheter som kör Android i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="10641-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="10641-106">Lägga till Wi-Fi-inställningar för Android Enterprise-dedikerade och fullständigt hanterade enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="10641-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="10641-107">Lägga till Wi-Fi-inställningar för iOS- och iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="10641-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="10641-108">Lägga till Wi-Fi-inställningar för Windows 10 och senare enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="10641-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="10641-109">Importera Wi-Fi-inställningar för Windows-enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="10641-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="10641-110">**Vanliga frågor**</span><span class="sxs-lookup"><span data-stu-id="10641-110">**Common Issues**</span></span>

<span data-ttu-id="10641-111">**Jag distribuerar en Wi-Fi-profil som är beroende av ett distribuerat certifikat som anges i Wi-Fi-profilen. Konfigurationsprofilerna visar dock en felstatus.**</span><span class="sxs-lookup"><span data-stu-id="10641-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="10641-112">Kontrollera att enheten har tagit emot certifikatet.</span><span class="sxs-lookup"><span data-stu-id="10641-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="10641-113">Gå till **Alla enheter** i Intune och välj **enhetskonfigurationen**> enhet .</span><span class="sxs-lookup"><span data-stu-id="10641-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="10641-114">Kontrollera att alla förväntade profiler visas och i ett framgångsrikt tillstånd.</span><span class="sxs-lookup"><span data-stu-id="10641-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="10641-115">Om du har mellanliggande certifikat i certifikatkedjan för en Android-profil kontrollerar du att de distribueras till Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="10641-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="10641-116">Om du vill kontrollera certifikatstatusen går du till **Enhetskonfigurationsprofiler**  >  **Profiles**  >  **android mellanliggande certifikatutfärdaregenskaper**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="10641-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="10641-117">Om du fortsätter att se fel läser du procedurerna och felsökningsavsnitten.</span><span class="sxs-lookup"><span data-stu-id="10641-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="10641-118">Mer information finns i [Översikt för felsökning av SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="10641-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="10641-119">**Jag har distribuerat en Wi-Fi-profil till en enhet. Intune visar att det lyckades, men enheten ansluter inte till Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="10641-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="10641-120">En lyckad status innebär att Intune har distribuerat profilen som konfigurerad.</span><span class="sxs-lookup"><span data-stu-id="10641-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="10641-121">Dessa konfigurationer kanske inte matchar dina nätverks- och/eller autentiseringskrav.</span><span class="sxs-lookup"><span data-stu-id="10641-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="10641-122">Mer information om anslutningens försök finns i infrastruktur- och autentiseringstjänsten (på Wi-Fi-åtkomstpunktsstyrenheten och NPS/Radius-servern).</span><span class="sxs-lookup"><span data-stu-id="10641-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="10641-123">Du kanske måste arbeta med nätverksinfrastrukturteamet, eller wi-fi-leverantören från tredje part, för att samla in och granska loggar.</span><span class="sxs-lookup"><span data-stu-id="10641-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>