---
title: Hindra meddelanden från att flyttas till arkivet automatiskt
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
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527117"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="17eaf-102">Hindra meddelanden från att flyttas till arkivet automatiskt</span><span class="sxs-lookup"><span data-stu-id="17eaf-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="17eaf-103">Om du använder en bevarandeprincip kan du ändra bevarandeåldern i principen så att meddelanden inte arkiveras automatiskt.</span><span class="sxs-lookup"><span data-stu-id="17eaf-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="17eaf-104">Så här gör du:</span><span class="sxs-lookup"><span data-stu-id="17eaf-104">Here's how:</span></span>

1. <span data-ttu-id="17eaf-105">Välj [bevarandetaggar för efterlevnadshantering](https://go.microsoft.com/fwlink/?linkid=2059104) **i**  >  **administrationscentret för** Exchange.</span><span class="sxs-lookup"><span data-stu-id="17eaf-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="17eaf-106">Leta reda på bevarandetaggen Flytta till arkiv.</span><span class="sxs-lookup"><span data-stu-id="17eaf-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="17eaf-107">Ändra bevarandetiden (arkivperioden) i bevarandetaggen till Aldrig för att förhindra att objekt automatiskt arkiveras av en bevarandeprincip. </span><span class="sxs-lookup"><span data-stu-id="17eaf-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="17eaf-108">Det här ändrar arkivinställningen för alla postlådor där den här bevarandetaggen används för dem.</span><span class="sxs-lookup"><span data-stu-id="17eaf-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
