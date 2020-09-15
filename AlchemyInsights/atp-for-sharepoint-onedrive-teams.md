---
title: ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715579"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="67f21-102">ATP för SharePoint, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="67f21-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="67f21-103">Följ de här anvisningarna för att aktivera avancerat skydd:</span><span class="sxs-lookup"><span data-stu-id="67f21-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="67f21-104">Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhets administratörs konto.</span><span class="sxs-lookup"><span data-stu-id="67f21-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="67f21-105">I det vänstra navigerings fönstret under **Threat Management**väljer du **policy** \> **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="67f21-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="67f21-106">Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="67f21-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="67f21-107">[Skapa en aktivitets aviserings princip](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) för att få aviseringar när vi upptäcker skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="67f21-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="67f21-108">Anvisningar finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="67f21-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="67f21-109">**Obs!** med ATP genomsöks inte alla filer i SharePoint Online, OneDrive för företag eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="67f21-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="67f21-110">Filer skannas asynkront av en process som använder delnings aktivitet, gäst aktivitet och hot signaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="67f21-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="67f21-111">Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="67f21-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
