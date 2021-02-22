---
title: Dölj gemensamma mappar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315441"
---
# <a name="hide-public-folders"></a><span data-ttu-id="ea7fc-102">Dölj gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="ea7fc-102">Hide public folders</span></span>

<span data-ttu-id="ea7fc-103">**Så här döljer du hela träd i den gemensamma mappen:**</span><span class="sxs-lookup"><span data-stu-id="ea7fc-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="ea7fc-104">Använd stegen i den [här artikeln](https://aka.ms/ControlPF) för att dölja hela offentliga mappträd för selektiva eller alla användare.</span><span class="sxs-lookup"><span data-stu-id="ea7fc-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="ea7fc-105">**Så här döljer du en specifik offentlig mapp:**</span><span class="sxs-lookup"><span data-stu-id="ea7fc-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="ea7fc-106">Lägga till behörigheter för användare som behöver åtkomst till den gemensamma mappen</span><span class="sxs-lookup"><span data-stu-id="ea7fc-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="ea7fc-107">Ta bort **användarens standard** från **behörighetslistan:**</span><span class="sxs-lookup"><span data-stu-id="ea7fc-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
