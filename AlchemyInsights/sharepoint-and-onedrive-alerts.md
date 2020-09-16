---
title: Fördröjningar vid mottagning av SharePoint-och OneDrive-aviseringar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727261"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="9077c-102">Fördröjningar vid mottagning av SharePoint-och OneDrive-aviseringar</span><span class="sxs-lookup"><span data-stu-id="9077c-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="9077c-103">Kontrol lera först skräppostmappen i e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="9077c-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="9077c-104">Om **alla aviseringar från flera filer eller bibliotek är försenade**kan du gå till [instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home?ref=/servicehealth) för att söka efter eventuella rådgivare/händelser som kan komma att inträffa med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="9077c-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="9077c-105">Problemet kan bero på SharePoint-aviseringens kapacitet eller fördröjningar i e-postmeddelanden via Exchange.</span><span class="sxs-lookup"><span data-stu-id="9077c-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="9077c-106">Observera även om andra e-postmeddelanden levereras – om det inte är det beror problemet sannolikt på Exchange-fördröjningar.</span><span class="sxs-lookup"><span data-stu-id="9077c-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="9077c-107">Om **en enskild avisering från en viss fil eller ett visst bibliotek inte levereras**försöker du ta bort och återskapa den.</span><span class="sxs-lookup"><span data-stu-id="9077c-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="9077c-108">Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.</span><span class="sxs-lookup"><span data-stu-id="9077c-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="9077c-109">Det går inte att skicka aviseringar till en distributions grupp.</span><span class="sxs-lookup"><span data-stu-id="9077c-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="9077c-110">Endast säkerhets-och O365-grupper stöds.</span><span class="sxs-lookup"><span data-stu-id="9077c-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="9077c-111">Du kan inte anpassa e-postmallar för aviseringar.</span><span class="sxs-lookup"><span data-stu-id="9077c-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="9077c-112">Du måste använda Microsoft Flow eller SharePoint Designer-arbetsflöde för att få dem.</span><span class="sxs-lookup"><span data-stu-id="9077c-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
