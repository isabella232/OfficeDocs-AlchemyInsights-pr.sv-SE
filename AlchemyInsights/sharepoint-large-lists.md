---
title: Omfattande SharePoint-listor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720151"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="ee483-102">Arbeta med stora listor och bibliotek i SharePoint</span><span class="sxs-lookup"><span data-stu-id="ee483-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="ee483-103">SharePoint-listor och-bibliotek kan innehålla upp till 30 000 000 objekt, men när de har mer än 5 000 objekt kanske ett fel meddelande visas när du försöker arbeta med dem.</span><span class="sxs-lookup"><span data-stu-id="ee483-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="ee483-104">Tröskelvärdet är till för att upprätthålla tjänstens prestanda.</span><span class="sxs-lookup"><span data-stu-id="ee483-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="ee483-105">Det kan inte ändras.</span><span class="sxs-lookup"><span data-stu-id="ee483-105">It can't be changed.</span></span> <span data-ttu-id="ee483-106">För att undvika att det här tröskelvärdet uppnåddes:</span><span class="sxs-lookup"><span data-stu-id="ee483-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="ee483-107">**Använd moderna**</span><span class="sxs-lookup"><span data-stu-id="ee483-107">**Use modern**</span></span>

<span data-ttu-id="ee483-108">Vyer som visar många objekt fungerar bäst i den moderna upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee483-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="ee483-109">[Använd den moderna upplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) för att undvika fel som kan uppstå i den klassiska upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="ee483-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="ee483-110">**Lägga till index**</span><span class="sxs-lookup"><span data-stu-id="ee483-110">**Add indexes**</span></span>

<span data-ttu-id="ee483-111">När du filtrerar eller sorterar efter en kolumn som inte har ett index kanske du får ett fel meddelande.</span><span class="sxs-lookup"><span data-stu-id="ee483-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="ee483-112">[Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt från **list inställningar** på menyn Inställningar och sedan **indexerade kolumner**.</span><span class="sxs-lookup"><span data-stu-id="ee483-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="ee483-113">**Redigera listvyn**</span><span class="sxs-lookup"><span data-stu-id="ee483-113">**Edit the list view**</span></span>

<span data-ttu-id="ee483-114">Om det uppstår ett fel när du arbetar med en stor lista [redigerar du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="ee483-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="ee483-115">Följande fyra ändringar tar bort tröskelvärden för listvyer.</span><span class="sxs-lookup"><span data-stu-id="ee483-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="ee483-116">Gör alla fyra ändringar för att ta bort alla fel.</span><span class="sxs-lookup"><span data-stu-id="ee483-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="ee483-117">Om du fortfarande får fel meddelanden markerar du [hantera stora listor och bibliotek](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="ee483-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="ee483-118">Välj **ingen** från **den första sorteringen efter kolumnen** och **Sortera sedan efter kolumnen**.</span><span class="sxs-lookup"><span data-stu-id="ee483-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="ee483-119">Välj **ingen** från **den första gruppen efter kolumnen** och **Gruppera sedan efter kolumnen**.</span><span class="sxs-lookup"><span data-stu-id="ee483-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="ee483-120">Välj **ingen** för alla kolumner i avsnittet **summor** .</span><span class="sxs-lookup"><span data-stu-id="ee483-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="ee483-121">Avmarkera alla **kolumner** utom en i kolumnerna.</span><span class="sxs-lookup"><span data-stu-id="ee483-121">Deselect all but one column for display from the **Columns** section.</span></span>

