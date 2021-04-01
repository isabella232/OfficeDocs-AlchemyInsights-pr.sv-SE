---
title: Ange Microsoft Edge som standardwebbläsare på en macOS-enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491816"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="d9eab-102">Ange Microsoft Edge som standardwebbläsare på en macOS-enhet</span><span class="sxs-lookup"><span data-stu-id="d9eab-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="d9eab-103">Använd någon av de här två metoderna för att ange Microsoft Edge som standardwebbläsare:</span><span class="sxs-lookup"><span data-stu-id="d9eab-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="d9eab-104">Metod 1: Flasha enheten med en bild av macOS där Microsoft Edge redan har angetts som standardwebbläsare.</span><span class="sxs-lookup"><span data-stu-id="d9eab-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="d9eab-105">Metod 2: Ställ in principen DefaultBrowserSettingEnabled så att användaren uppmanas att ange Microsoft Edge som standardwebbläsare.</span><span class="sxs-lookup"><span data-stu-id="d9eab-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="d9eab-106">Oavsett vilken metod du använder kan användaren ändra standardwebbläsaren.</span><span class="sxs-lookup"><span data-stu-id="d9eab-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="d9eab-107">Därför rekommenderar vi att du använder principen DefaultBrowserSettingEnabled även om du använder metod 1.</span><span class="sxs-lookup"><span data-stu-id="d9eab-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="d9eab-108">Om en användare ändrar standardwebbläsaren efter att principen har distribuerats uppmanas användaren att ställa in standardwebbläsaren till Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d9eab-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
