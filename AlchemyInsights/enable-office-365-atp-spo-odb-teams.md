---
title: Aktivera Office 365 ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506936"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="051fe-102">Aktivera avancerat skydd mot office 365 för SharePoint Online, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="051fe-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="051fe-103">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="051fe-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="051fe-104">Välj Säkra bilagor **för**  >  **Policy**  >  **hothanteringsprincip .**</span><span class="sxs-lookup"><span data-stu-id="051fe-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="051fe-105">Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**och klicka sedan på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="051fe-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="051fe-106">(Rekommenderas) Som global administratör eller SharePoint Online-administratör kör du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** inställd på *true*.</span><span class="sxs-lookup"><span data-stu-id="051fe-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="051fe-107">(Rekommenderas) [Ställ in aviseringar](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.</span><span class="sxs-lookup"><span data-stu-id="051fe-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="051fe-108">ATP kommer att skanna varenda fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="051fe-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="051fe-109">Filer skannas asynkront, genom en process som använder delnings- och gästaktivitetshändelser, tillsammans med smarta heuristik och hotsignaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="051fe-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="051fe-110">Se [ATP för SharePoint, OneDrive och Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="051fe-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>