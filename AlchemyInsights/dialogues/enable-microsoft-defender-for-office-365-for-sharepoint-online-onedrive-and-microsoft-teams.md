---
title: Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695655"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4022b-102">Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4022b-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="4022b-103">Använd dina autentiseringsuppgifter som global administratör eller säkerhetsadministratör och logga in på Säkerhets- och [efterlevnadscenter för Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="4022b-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="4022b-104">Välj **Hothantering** i den vänstra rutan och välj **sedan** Policy Safe  >  [attachments.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="4022b-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="4022b-105">Välj **Aktivera Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams** och välj sedan **Spara.**</span><span class="sxs-lookup"><span data-stu-id="4022b-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="4022b-106">Som global administratör eller SharePoint Online-administratör kör du följande PowerShell-cmdlet med **parametern DisallowInfectedFileDownload** a true *:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="4022b-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="4022b-107">Konfigurera aviseringar för identifierade filer</span><span class="sxs-lookup"><span data-stu-id="4022b-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="4022b-108">Mer information finns i [Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="4022b-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
