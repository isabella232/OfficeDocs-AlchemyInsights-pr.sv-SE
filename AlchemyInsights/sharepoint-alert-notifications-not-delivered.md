---
title: SharePoint-aviseringar skickas inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751261"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="5a104-102">SharePoint-aviseringar skickas inte</span><span class="sxs-lookup"><span data-stu-id="5a104-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="5a104-103">Kontrol lera mappen skräp post i e-postmeddelandet, så snart meddelanden kan komma dit.</span><span class="sxs-lookup"><span data-stu-id="5a104-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="5a104-104">Avgöra om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.</span><span class="sxs-lookup"><span data-stu-id="5a104-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="5a104-105">**Enskilda meddelanden levereras inte**: om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den.</span><span class="sxs-lookup"><span data-stu-id="5a104-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="5a104-106">Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.</span><span class="sxs-lookup"><span data-stu-id="5a104-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="5a104-107">**Alla notifieringar levereras inte**: om alla aviseringar från flera filer eller bibliotek inte levereras kan du gå till [instrument panelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att söka efter eventuella rådgivare/händelser som kan komma att inträffa med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a104-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="5a104-108">Problemet kan uppstå med aviserings kapaciteten för SharePoint eller fördröjningar i e-postmeddelanden via Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a104-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="5a104-109">Det är också viktigt att notera om andra e-postmeddelanden levereras och om så inte är fallet beror problemet sannolikt på Exchange-fördröjningar.</span><span class="sxs-lookup"><span data-stu-id="5a104-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="5a104-110">Vanliga frågor och svar:</span><span class="sxs-lookup"><span data-stu-id="5a104-110">FAQ on alerts:</span></span>

- <span data-ttu-id="5a104-111">Det går inte att skicka meddelanden till distributions gruppen, endast säkerhets-och O365-grupper stöds.</span><span class="sxs-lookup"><span data-stu-id="5a104-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="5a104-112">Du kan inte anpassa e-postmallar för aviseringar; Du måste använda Microsoft FLOW eller SharePoint Designer-arbetsflöde för att få dem.</span><span class="sxs-lookup"><span data-stu-id="5a104-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="5a104-113">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="5a104-113">Related Topics</span></span>

<span data-ttu-id="5a104-114">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5a104-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="5a104-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="5a104-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="5a104-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="5a104-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
