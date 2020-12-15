---
title: Använda Microsoft Intune för att hantera Internet åtkomst i Microsoft Edge för iOS och Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679609"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="21d61-102">Använda Microsoft Intune för att hantera Internet åtkomst i Microsoft Edge för iOS och Android</span><span class="sxs-lookup"><span data-stu-id="21d61-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="21d61-103">Med Microsoft Edge för iOS och Android kan en användare surfa på webben från flera, helt separata profiler.</span><span class="sxs-lookup"><span data-stu-id="21d61-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="21d61-104">De bredaste skydds funktionerna för Microsoft 365-data blir tillgängliga när du abonnerar på företags mobilitet + säkerhets paketet, som innehåller Microsoft Intune och Azure Active Directory Premium-funktioner, till exempel villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="21d61-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="21d61-105">Ett minimum är att du vill distribuera en princip för villkorsstyrd åtkomst som (1) låter användare ansluta från mobila enheter till Microsoft Edge för iOS och Android och det (2) implementerar en Microsoft Intune App-Protection-princip som ger en skyddad webbläsare.</span><span class="sxs-lookup"><span data-stu-id="21d61-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="21d61-106">Information om hur du kan använda villkorsstyrd åtkomst och principer finns i:</span><span class="sxs-lookup"><span data-stu-id="21d61-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="21d61-107">Tillämpa principer för villkorsstyrd åtkomst för Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="21d61-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="21d61-108">Skapa säkerhets principer för Microsoft Intune-appar</span><span class="sxs-lookup"><span data-stu-id="21d61-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="21d61-109">Använda enkel inloggning för Azure Active Directory – anslutna webb program i lösenordsskyddade webbläsare</span><span class="sxs-lookup"><span data-stu-id="21d61-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="21d61-110">Använd program konfigurationen för att hantera webbläsaren</span><span class="sxs-lookup"><span data-stu-id="21d61-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="21d61-111">Tillåt endast arbets-och skol konton</span><span class="sxs-lookup"><span data-stu-id="21d61-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="21d61-112">Distribuera allmänna konfigurations principer för appar</span><span class="sxs-lookup"><span data-stu-id="21d61-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="21d61-113">Distribuera konfigurations principer för appar för data skydd</span><span class="sxs-lookup"><span data-stu-id="21d61-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="21d61-114">Använda Microsoft Endpoint Manager för att distribuera program konfigurations principer</span><span class="sxs-lookup"><span data-stu-id="21d61-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="21d61-115">Information om hur du kommer åt hanterade program loggar finns i [använda Microsoft Edge för iOS och Android för att komma åt hanterade program loggar](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="21d61-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
