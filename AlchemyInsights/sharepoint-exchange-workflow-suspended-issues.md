---
title: Komma igång med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700725"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="8e611-102">Arbets flöden i SharePoint</span><span class="sxs-lookup"><span data-stu-id="8e611-102">Workflows in SharePoint</span></span>

<span data-ttu-id="8e611-103">Om det inte går att skicka e-post från SharePoint-arbetsflöden kan din organisation ha påträffat begränsningar för Exchange Online-avsändaren.</span><span class="sxs-lookup"><span data-stu-id="8e611-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="8e611-104">Fel meddelandet "arbets flödet är upptaget" kan visas om du har något av följande:</span><span class="sxs-lookup"><span data-stu-id="8e611-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="8e611-105">Du har ett arbets flöde i SharePoint Online som använder plattforms typen SharePoint 2010 eller SharePoint 2013 Workflow Platform.</span><span class="sxs-lookup"><span data-stu-id="8e611-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="8e611-106">Arbets flödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="8e611-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="8e611-107">När du kör arbets flödet skickas inte e-postmeddelandet, och du märker att fel meddelandet, att intern status är inaktive rad eller inte kan skicka till en mottagare visas.</span><span class="sxs-lookup"><span data-stu-id="8e611-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="8e611-108">Mer information finns i följande [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="8e611-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

