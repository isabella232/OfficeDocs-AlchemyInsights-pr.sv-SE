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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709925"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="16c97-102">Aktivera Office 365 Avancerat skydd för SharePoint Online, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="16c97-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="16c97-103">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="16c97-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="16c97-104">Välj **hot Management**  >  **policy**-  >  **säkra bifogade filer**.</span><span class="sxs-lookup"><span data-stu-id="16c97-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="16c97-105">Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**och klicka sedan på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="16c97-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="16c97-106">Lämpligt Som global administratör eller SharePoint Online-administratör kör du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** angiven till *True*.</span><span class="sxs-lookup"><span data-stu-id="16c97-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="16c97-107">Lämpligt [Konfigurera aviseringar](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.</span><span class="sxs-lookup"><span data-stu-id="16c97-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="16c97-108">ATP kan du söka igenom alla filer i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16c97-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="16c97-109">Filer skannas asynkront, genom en process där delnings-och gäst aktivitets händelser används tillsammans med smarta heuristik och hot signaler.</span><span class="sxs-lookup"><span data-stu-id="16c97-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="16c97-110">Se [ATP för SharePoint, OneDrive och Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="16c97-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>