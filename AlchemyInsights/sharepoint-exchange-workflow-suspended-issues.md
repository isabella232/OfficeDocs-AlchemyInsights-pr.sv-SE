---
title: Kom igång med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051659"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="b298e-102">Arbetsflöden i SharePoint</span><span class="sxs-lookup"><span data-stu-id="b298e-102">Workflows in SharePoint</span></span>

<span data-ttu-id="b298e-103">Om SharePoint-arbetsflöden inte skickar e-post, kan din organisation har stött på Exchange Online avsändar gränser.</span><span class="sxs-lookup"><span data-stu-id="b298e-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="b298e-104">Felmeddelandet "arbetsflöde är pausad" kan uppstå om du har något av följande:</span><span class="sxs-lookup"><span data-stu-id="b298e-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="b298e-105">Du har ett arbetsflöde i SharePoint Online som använder den SharePoint 2010 eller SharePoint 2013 arbetsflödestyp plattform.</span><span class="sxs-lookup"><span data-stu-id="b298e-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="b298e-106">Arbetsflödet har konfigurerats för att skicka ett anpassat e-postmeddelande till mer än 200 användare i taget, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="b298e-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="b298e-107">När du kör arbetsflödet e-postmeddelandet skickas inte och du märker felmeddelandet, intern status är inställd på pausad eller det går inte att skicka till en mottagare visas.</span><span class="sxs-lookup"><span data-stu-id="b298e-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="b298e-108">För mer information, se följande [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="b298e-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

