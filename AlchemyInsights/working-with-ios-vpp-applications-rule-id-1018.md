---
title: Arbeta med iOS VPP program regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364887"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="72212-102">Arbeta med iOS VPP program</span><span class="sxs-lookup"><span data-stu-id="72212-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="72212-103">Läsa om [hur du hanterar iOS-appar som köpts via en inköpsvolym program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) du lär dig mer om funktioner, villkor och åtgärder för att kontrollera användning av Apple volym köpa Program och stöd för den i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="72212-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="72212-104">**Vanliga problem:** ”Jag har tilldelat en VPP iOS-app för användarna, men installationen misslyckades”.</span><span class="sxs-lookup"><span data-stu-id="72212-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="72212-105">Detta kan inträffa om en enda VPP-token används över flera leverantörer för hantering av mobil enhet.</span><span class="sxs-lookup"><span data-stu-id="72212-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="72212-106">VPP-token från Apple kan endast användas med en provider.</span><span class="sxs-lookup"><span data-stu-id="72212-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="72212-107">Om du använde en VPP-token med flera leverantörer måste du överföra token till Intune.</span><span class="sxs-lookup"><span data-stu-id="72212-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="72212-108">Installationen misslyckas även om det totala antalet installationer av överskrider antalet licenser.</span><span class="sxs-lookup"><span data-stu-id="72212-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="72212-109">Om du vill visa en användningsrapport för din licens, gå till **Intune Mobile apps** \> **App licenser** sida.</span><span class="sxs-lookup"><span data-stu-id="72212-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="72212-110">Information om hur du frigör licenser används, se [i den här artikeln.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="72212-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
