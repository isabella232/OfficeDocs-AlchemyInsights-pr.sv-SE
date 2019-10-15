---
title: SharePoint stora listor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488535"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="4239c-102">Arbeta med stora listor och bibliotek i SharePoint</span><span class="sxs-lookup"><span data-stu-id="4239c-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="4239c-103">SharePoint-listor och-bibliotek kan innehålla upp till 30 000 000 objekt, men när de har fler än 5 000 objekt kan du se ett tröskelvärde för listvy-fel när du försöker arbeta med dem.</span><span class="sxs-lookup"><span data-stu-id="4239c-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="4239c-104">Det här tröskelvärdet är på plats för att upprätthålla tjänstens prestanda.</span><span class="sxs-lookup"><span data-stu-id="4239c-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="4239c-105">Det går inte att ändra.</span><span class="sxs-lookup"><span data-stu-id="4239c-105">It can't be changed.</span></span> <span data-ttu-id="4239c-106">Så här undviker du att träffa denna tröskel:</span><span class="sxs-lookup"><span data-stu-id="4239c-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="4239c-107">**Använda moderna**</span><span class="sxs-lookup"><span data-stu-id="4239c-107">**Use modern**</span></span>

<span data-ttu-id="4239c-108">Vyer som visar många objekt fungerar bäst i den moderna upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="4239c-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="4239c-109">[Använd den moderna upplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) för att undvika fel som du kan se i den klassiska upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="4239c-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="4239c-110">**Lägg till index**</span><span class="sxs-lookup"><span data-stu-id="4239c-110">**Add indexes**</span></span>

<span data-ttu-id="4239c-111">När du filtrerar eller sorterar efter en kolumn som inte har ett index kan ett felmeddelande visas.</span><span class="sxs-lookup"><span data-stu-id="4239c-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="4239c-112">[Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt från **list inställningar** på menyn Inställningar och sedan **indexerade kolumner**.</span><span class="sxs-lookup"><span data-stu-id="4239c-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="4239c-113">**Redigera listvyn**</span><span class="sxs-lookup"><span data-stu-id="4239c-113">**Edit the list view**</span></span>

<span data-ttu-id="4239c-114">Om ett fel uppstår när du arbetar med en stor lista [redigerar du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="4239c-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="4239c-115">Följande fyra ändringar tar bort fel i listvyns tröskelvärde.</span><span class="sxs-lookup"><span data-stu-id="4239c-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="4239c-116">Gör alla fyra ändringarna för att ta bort alla fel.</span><span class="sxs-lookup"><span data-stu-id="4239c-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="4239c-117">Om du fortfarande får fel, kontrollera [hantera stora listor och bibliotek](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="4239c-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="4239c-118">Välj **ingen** från båda **först sortera efter kolumnen** och **Sortera sedan efter kolumnen**.</span><span class="sxs-lookup"><span data-stu-id="4239c-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="4239c-119">Välj **ingen** från **den första gruppen i kolumnen** och **Gruppera sedan efter kolumnen**.</span><span class="sxs-lookup"><span data-stu-id="4239c-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="4239c-120">Välj **ingen** för alla kolumner i avsnittet **summor** .</span><span class="sxs-lookup"><span data-stu-id="4239c-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="4239c-121">Avmarkera alla utom en kolumn för visning från avsnittet **kolumner** .</span><span class="sxs-lookup"><span data-stu-id="4239c-121">Deselect all but one column for display from the **Columns** section.</span></span>

