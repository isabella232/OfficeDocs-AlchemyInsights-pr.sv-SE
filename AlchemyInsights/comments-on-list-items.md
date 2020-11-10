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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982556"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="cab0c-102">Kommentarer om List objekt</span><span class="sxs-lookup"><span data-stu-id="cab0c-102">Comments on List items</span></span>

<span data-ttu-id="cab0c-103">Användarna kan snart lägga till och ta bort kommentarer för List objekt.</span><span class="sxs-lookup"><span data-stu-id="cab0c-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="cab0c-104">Användare kan visa alla kommentarer på ett List objekt och filtrera mellan vyer som visar kommentarer eller aktiviteter relaterade till ett objekt.</span><span class="sxs-lookup"><span data-stu-id="cab0c-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="cab0c-105">**Tids inställning** :</span><span class="sxs-lookup"><span data-stu-id="cab0c-105">**Timing** :</span></span>

<span data-ttu-id="cab0c-106">**Riktad version** : successivt utgiven i Mid-oktober och förväntas bli färdig med Mid-november</span><span class="sxs-lookup"><span data-stu-id="cab0c-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="cab0c-107">**Standard version** : successivt utgiven i Mid-november och förväntas bli slutfört av tidigt december</span><span class="sxs-lookup"><span data-stu-id="cab0c-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="cab0c-108">**Rollout** Installation: riktad version för hela organisationen</span><span class="sxs-lookup"><span data-stu-id="cab0c-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="cab0c-109">Användare måste anteckna följande innan de kan lägga till och ta bort kommentarer:</span><span class="sxs-lookup"><span data-stu-id="cab0c-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="cab0c-110">Kommentarer följer de behörighets inställningar som finns i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cab0c-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="cab0c-111">Klassiska listor som ännu inte har byggts för att visas i moderna användar gränssnitt, som aktivitets listor, har inte den här kommentars funktionen.</span><span class="sxs-lookup"><span data-stu-id="cab0c-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="cab0c-112">Det går inte att kommentera listor i Teams med den här versionen.</span><span class="sxs-lookup"><span data-stu-id="cab0c-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="cab0c-113">Kommentarer indexeras inte efter sökning.</span><span class="sxs-lookup"><span data-stu-id="cab0c-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="cab0c-114">Administratörer kan inaktivera den här funktionen på organisations nivå genom att ändra parametern **CommentsOnListItemsDisabled** i PowerShell-cmdleten **Set-SPOTenant** .</span><span class="sxs-lookup"><span data-stu-id="cab0c-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="cab0c-115">Det går för närvarande inte att inaktivera kommentarer på webbplats-eller listnivå.</span><span class="sxs-lookup"><span data-stu-id="cab0c-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="cab0c-116">Vi hoppas att få dessa kontroller i en senare uppdatering, troligen i det första kvartalet 2021.</span><span class="sxs-lookup"><span data-stu-id="cab0c-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
