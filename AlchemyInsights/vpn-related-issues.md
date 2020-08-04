---
title: VPN-relaterade problem
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555744"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="f215b-102">VPN-relaterade problem</span><span class="sxs-lookup"><span data-stu-id="f215b-102">VPN related issues</span></span>

<span data-ttu-id="f215b-103">En lyckad implementering av VPN-anslutning för MDM-klienter beror på en distribuerad profil som korrekt återspeglar kraven för VPN-infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="f215b-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="f215b-104">För lämpliga inställningar för klientplattformarna som du undersöker finns i:</span><span class="sxs-lookup"><span data-stu-id="f215b-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="f215b-105">Inställningar för Windows 10 och Windows Holographic device för att lägga till VPN-anslutningar med Intune</span><span class="sxs-lookup"><span data-stu-id="f215b-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="f215b-106">Lägga till VPN-inställningar på iOS- och iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f215b-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="f215b-107">Inställningar för Android-enhet för att konfigurera VPN i Intune</span><span class="sxs-lookup"><span data-stu-id="f215b-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="f215b-108">Lägga till VPN-inställningar på macOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f215b-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="f215b-109">Om din VPN-profil använder certifikatbaserad autentisering kontrollerar du att rotcertifikat- och klientautentiseringscertifikatprofilerna som är länkade till VPN-profilen har distribuerats.</span><span class="sxs-lookup"><span data-stu-id="f215b-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="f215b-110">**Vanliga frågor**</span><span class="sxs-lookup"><span data-stu-id="f215b-110">**Common Issues**</span></span>

<span data-ttu-id="f215b-111">**Jag har distribuerat en VPN-profil till en enhet. Intune visar att det lyckades, men enheten ansluter inte till VPN.**</span><span class="sxs-lookup"><span data-stu-id="f215b-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="f215b-112">En lyckad status innebär att Intune har distribuerat profilen som konfigurerad.</span><span class="sxs-lookup"><span data-stu-id="f215b-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="f215b-113">Dessa konfigurationer kanske inte matchar dina nätverks- och/eller autentiseringskrav.</span><span class="sxs-lookup"><span data-stu-id="f215b-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="f215b-114">Granska loggar i infrastruktur- och autentiseringstjänsten (på VPN-servern och NPS/Radius-servern) för mer information om anslutningen.</span><span class="sxs-lookup"><span data-stu-id="f215b-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="f215b-115">Du kan behöva arbeta med nätverksinfrastrukturteamet, eller VPN-leverantören från tredje part, för att samla in och granska loggar.</span><span class="sxs-lookup"><span data-stu-id="f215b-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="f215b-116">**När jag konfigurerar en anpassad VPN för iOS görs VPN-funktionen per app inte tillgänglig.**</span><span class="sxs-lookup"><span data-stu-id="f215b-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="f215b-117">Vpn per app för iOS-enheter i Intune är för närvarande tillgängligt för en specifik lista över leverantörer och partner, som också måste uppfylla certifikatkraven innan du konfigurerar en VPN per app.</span><span class="sxs-lookup"><span data-stu-id="f215b-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="f215b-118">Mer information finns i [Konfigurera vpn (Virtual Private Network) per app för iOS/iPadOS-enheter i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="f215b-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="f215b-119">Mer information om alla VPN-anslutningstyper i Intune finns i [Skapa VPN-profiler för att ansluta till VPN-servrar i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="f215b-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="f215b-120">**iOS On-Demand VPN utlöses inte när en konfigurerad domän används**</span><span class="sxs-lookup"><span data-stu-id="f215b-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="f215b-121">Om du vill testa automatiska VPN-inställningar ställer du in följande värden:</span><span class="sxs-lookup"><span data-stu-id="f215b-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="f215b-122">Jag vill göra följande: **Utvärdera varje anslutningsförsök**</span><span class="sxs-lookup"><span data-stu-id="f215b-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="f215b-123">Välj om du vill ansluta: **Anslut om det behövs**</span><span class="sxs-lookup"><span data-stu-id="f215b-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="f215b-124">När användare kommer åt dessa domäner: **target** *måldomännamn*</span><span class="sxs-lookup"><span data-stu-id="f215b-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="f215b-125">Om ovanstående konfiguration inte lyckas lägger du till följande element:</span><span class="sxs-lookup"><span data-stu-id="f215b-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="f215b-126">När den här webbadressen inte kan nås tvingar du till VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="f215b-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>