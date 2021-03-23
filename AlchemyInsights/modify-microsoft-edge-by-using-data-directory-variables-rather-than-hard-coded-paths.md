---
title: Ändra Microsoft Edge med hjälp av datakatalogvariabler i stället för hårdkodade sökvägar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036858"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="fe0ed-102">Ändra Microsoft Edge med hjälp av datakatalogvariabler i stället för hårdkodade sökvägar</span><span class="sxs-lookup"><span data-stu-id="fe0ed-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="fe0ed-103">Om du till exempel i Windows vill lagra profildata under en användares lokala programdata i stället för på standardplatsen ställer du in *UserDataDir-principen* på **${local_app_data}\Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="fe0ed-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="fe0ed-104">Mer information finns i Skapa [microsoft Edge användardatakatalogvariabler](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span><span class="sxs-lookup"><span data-stu-id="fe0ed-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>