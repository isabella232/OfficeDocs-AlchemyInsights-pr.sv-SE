---
title: Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543595"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="4c121-102">Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4c121-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="4c121-103">Följ anvisningarna för att aktivera Microsoft Defender för Office 365:</span><span class="sxs-lookup"><span data-stu-id="4c121-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="4c121-104">Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhetsadministratörskonto.</span><span class="sxs-lookup"><span data-stu-id="4c121-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="4c121-105">I det vänstra navigeringsfönstret under **Hothantering** väljer du **Policy för** \> **Valv bilagor**.</span><span class="sxs-lookup"><span data-stu-id="4c121-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="4c121-106">Välj **Aktivera Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="4c121-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="4c121-107">[Skapa en princip för aktivitetsavisering](/microsoft-365/compliance/create-activity-alerts) för att få aviseringar när vi upptäcker skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="4c121-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="4c121-108">Fullständiga instruktioner finns i aktivera [aktivera Valv för SharePoint, OneDrive och Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="4c121-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="4c121-109">**Obs!** Som design söker inte Microsoft Defender för Office 365 igenom alla filer i SharePoint Online, OneDrive för företag eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4c121-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="4c121-110">Filer genomsöks asynkront av en process som använder delningsaktivitet, gästaktivitet och hot-signaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="4c121-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="4c121-111">Mer information finns i Bifoga [Valv för SharePoint, OneDrive och Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="4c121-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
