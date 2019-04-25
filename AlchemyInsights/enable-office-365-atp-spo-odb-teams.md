---
title: Aktivera Office 365 tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403051"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b3381-102">Aktivera Office 365 avancerade Threat Protection for SharePoint Online, OneDrive och Microsoft-team</span><span class="sxs-lookup"><span data-stu-id="b3381-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="b3381-103">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="b3381-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="b3381-104">Välj **Threat management** > **Policy** > **Säkra bifogade filer**.</span><span class="sxs-lookup"><span data-stu-id="b3381-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="b3381-105">Markera **Aktivera ATP för SharePoint, OneDrive, och Microsoft team**och klicka sedan på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="b3381-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="b3381-106">(Rekommenderas) Som global administratör eller en SharePoint Online-administratör som kör cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** har värdet *true*.</span><span class="sxs-lookup"><span data-stu-id="b3381-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="b3381-107">(Rekommenderas) [Ställ in varningar](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.</span><span class="sxs-lookup"><span data-stu-id="b3381-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="b3381-108">ATP kommer nFör skanna varje enskild fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b3381-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="b3381-109">Filer genomsöks asynkront, genom en process som använder fildelning och Gäst aktivitetshändelser, intelligent heuristik och hot-signaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="b3381-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="b3381-110">Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="b3381-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>