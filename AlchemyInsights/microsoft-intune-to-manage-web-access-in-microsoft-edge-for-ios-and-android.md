---
title: Använda Microsoft Intune för att hantera webbåtkomst i Microsoft Edge för iOS och Android
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
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989722"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1efbb-102">Använda Microsoft Intune för att hantera webbåtkomst i Microsoft Edge för iOS och Android</span><span class="sxs-lookup"><span data-stu-id="1efbb-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1efbb-103">Med Microsoft Edge för iOS och Android kan en användare surfa på webben från flera, helt separata profiler.</span><span class="sxs-lookup"><span data-stu-id="1efbb-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1efbb-104">De bredaste skyddsfunktionerna för Microsoft 365-data blir tillgängliga när du prenumererar på Enterprise Mobility + Security-paketet, som omfattar Microsoft Intune- och Azure Active Directory Premium-funktioner, till exempel villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="1efbb-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1efbb-105">Som ett minimum bör du distribuera en princip för villkorsstyrd åtkomst som (1) låter användare ansluta från mobila enheter till Microsoft Edge för iOS och Android och som (2) implementerar en appskyddsprincip för Microsoft Intune som ger en skyddad webbupplevelse.</span><span class="sxs-lookup"><span data-stu-id="1efbb-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1efbb-106">Information om hur du kan använda villkorsstyrd åtkomst och principer finns i:</span><span class="sxs-lookup"><span data-stu-id="1efbb-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1efbb-107">Använda villkorsstyrda åtkomstprinciper i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1efbb-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1efbb-108">Skapa appskyddsprinciper för Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1efbb-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1efbb-109">Använda enkel inloggning för Azure Active Directory-anslutna webbappar i principskyddade webbläsare</span><span class="sxs-lookup"><span data-stu-id="1efbb-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1efbb-110">Använda programkonfiguration för att hantera surfupplevelsen</span><span class="sxs-lookup"><span data-stu-id="1efbb-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1efbb-111">Tillåt endast användning av arbets- och skolkonton</span><span class="sxs-lookup"><span data-stu-id="1efbb-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1efbb-112">Distribuera allmänna principer för programkonfiguration</span><span class="sxs-lookup"><span data-stu-id="1efbb-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1efbb-113">Distribuera principer för programkonfiguration för dataskydd</span><span class="sxs-lookup"><span data-stu-id="1efbb-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1efbb-114">Använda Microsoft Endpoint Manager för att distribuera principer för programkonfiguration</span><span class="sxs-lookup"><span data-stu-id="1efbb-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1efbb-115">Mer information om hur du kommer åt hanterade apploggar finns [i Använda Microsoft Edge för iOS och Android för att komma åt hanterade apploggar.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="1efbb-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
