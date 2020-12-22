---
title: Kommentarer om List objekt
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
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724172"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="5edcc-102">Kommentarer om List objekt</span><span class="sxs-lookup"><span data-stu-id="5edcc-102">Comments on List items</span></span>

<span data-ttu-id="5edcc-103">Användare kan visa alla kommentarer på ett List objekt och filtrera mellan vyer som visar kommentarer eller aktiviteter relaterade till ett objekt.</span><span class="sxs-lookup"><span data-stu-id="5edcc-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="5edcc-104">Användare måste anteckna följande innan de kan lägga till och ta bort kommentarer:</span><span class="sxs-lookup"><span data-stu-id="5edcc-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="5edcc-105">Kommentarer följer de behörighets inställningar som finns i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5edcc-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="5edcc-106">Klassiska listor som ännu inte har byggts för att visas i moderna användar gränssnitt, som aktivitets listor, har inte den här kommentars funktionen.</span><span class="sxs-lookup"><span data-stu-id="5edcc-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="5edcc-107">Det går inte att kommentera listor i Teams med den här versionen.</span><span class="sxs-lookup"><span data-stu-id="5edcc-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="5edcc-108">Kommentarer indexeras inte efter sökning.</span><span class="sxs-lookup"><span data-stu-id="5edcc-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="5edcc-109">Administratörer kan inaktivera den här funktionen på organisations nivå genom att ändra parametern **CommentsOnListItemsDisabled** i PowerShell-cmdleten **Set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="5edcc-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="5edcc-110">Det går för närvarande inte att inaktivera kommentarer på webbplats-eller listnivå.</span><span class="sxs-lookup"><span data-stu-id="5edcc-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="5edcc-111">Vi hoppas att få dessa kontroller i en senare uppdatering, troligen i det första kvartalet 2021.</span><span class="sxs-lookup"><span data-stu-id="5edcc-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
