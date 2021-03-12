---
title: Stoppa meddelanden från att flyttas till arkivet automatiskt
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749819"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="a58aa-102">Stoppa meddelanden från att flyttas till arkivet automatiskt</span><span class="sxs-lookup"><span data-stu-id="a58aa-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="a58aa-103">Om du använder en bevarandeprincip kan du ändra bevarandeåldern i den principen om du inte vill att meddelandena ska arkiveras automatiskt.</span><span class="sxs-lookup"><span data-stu-id="a58aa-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="a58aa-104">Så här gör du:</span><span class="sxs-lookup"><span data-stu-id="a58aa-104">Here's how:</span></span>

1. <span data-ttu-id="a58aa-105">Välj [bevarandetaggar för efterlevnadshantering](https://go.microsoft.com/fwlink/?linkid=2059104) **i** Exchange  >  **admin center.**</span><span class="sxs-lookup"><span data-stu-id="a58aa-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="a58aa-106">Leta reda på bevarandetaggen Flytta till arkiv.</span><span class="sxs-lookup"><span data-stu-id="a58aa-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="a58aa-107">Ändra kvarhållningstiden (arkiveringstiden) i  bevarandetaggen till Aldrig för att hindra att objekt automatiskt arkiveras av en bevarandeprincip.</span><span class="sxs-lookup"><span data-stu-id="a58aa-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="a58aa-108">Det här ändrar inställningen för arkivering för alla postlådor där den här bevarandetaggen används för dem.</span><span class="sxs-lookup"><span data-stu-id="a58aa-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
