---
title: MC210173 – SharePoint Designer nytt anpassat formulär funktion utfasning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831824"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="76ece-102">MC210173 – SharePoint Designer nytt anpassat formulär funktion utfasning</span><span class="sxs-lookup"><span data-stu-id="76ece-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="76ece-103">Vi har identifierat ett problem som påverkar SharePoint Designer-funktionerna för [att skapa anpassade formulär](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="76ece-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="76ece-104">Efter noggrann undersökning har vi fastställt att det inte finns någon känd lösning på problemet och valt att inaktivera funktionen för att skapa anpassade formulär effektivt fr. 3:00 AM UTC på lördag, 25 april 2020.</span><span class="sxs-lookup"><span data-stu-id="76ece-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="76ece-105">Den här ändringen påverkar inte möjligheten att redigera tidigare skapade formulär och andra befintliga funktioner i SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="76ece-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="76ece-106">När du har gjort det kan användarna få följande felmeddelande: "Det gick inte att spara liständringarna på servern" när du skapar nya formulär.</span><span class="sxs-lookup"><span data-stu-id="76ece-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="76ece-107">Användare som tidigare har använt SharePoint Designer för att skapa egna formulär kan i stället använda [PowerApps-](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) för det ändamålet.</span><span class="sxs-lookup"><span data-stu-id="76ece-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="76ece-108">PowerApps är ett enkelt och kraftfullt verktyg som gör det möjligt för användare i SharePoint Online Modern Experience att skapa och redigera anpassade formulär för SharePoint-listor och dokumentbibliotek direkt i ett webbläsarfönster.</span><span class="sxs-lookup"><span data-stu-id="76ece-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="76ece-109">PowerApps kräver inte traditionella koder eller att kunna koda eller några andra nedladdningar av appar som InfoPath.</span><span class="sxs-lookup"><span data-stu-id="76ece-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="76ece-110">**Obs**: användare av SharePoint Online Classic kommer tillfälligt att behöva gå över till den moderna miljön för att få tillgång till och använda PowerApps; alla anpassade formulär som skapas i PowerApps är dock tillgängliga för användare av SharePoint Online Classic Experience.</span><span class="sxs-lookup"><span data-stu-id="76ece-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
