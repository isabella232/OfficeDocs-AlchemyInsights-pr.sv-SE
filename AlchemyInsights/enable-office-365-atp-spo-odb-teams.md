---
title: Aktivera Office 365 ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543946"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="db952-102">Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="db952-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="db952-103">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="db952-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="db952-104">Välj **Policy för hantering** av  >  **hot** Valv bifogade  >  **filer.**</span><span class="sxs-lookup"><span data-stu-id="db952-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="db952-105">Välj **Aktivera Defender för Office 365 för SharePoint, OneDrive, Microsoft Teams** och klicka sedan på **Spara.**</span><span class="sxs-lookup"><span data-stu-id="db952-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="db952-106">(Rekommenderas) Som global administratör eller SharePoint Online-administratör kör du [cmdleten Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **parametern DisallowInfectedFileDownload** inställd på *sant.*</span><span class="sxs-lookup"><span data-stu-id="db952-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="db952-107">(Rekommenderas) [Konfigurera aviseringar för](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) identifierade filer.</span><span class="sxs-lookup"><span data-stu-id="db952-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="db952-108">Microsoft Defender för Office 365 genomsöker inte alla filer i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="db952-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="db952-109">Filer skannas asynkront genom en process som använder delning och gästaktivitetshändelser, tillsammans med smart heuristics och hot-signaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="db952-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="db952-110">Se [Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="db952-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>