---
title: Felsökning av Microsoft Defender för Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545286"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="f217a-102">Felsökning av Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="f217a-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="f217a-103">**Märker du fördröjningar i meddelandeleveransen?**</span><span class="sxs-lookup"><span data-stu-id="f217a-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="f217a-104">Använd alternativet [Dynamisk leverans](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i Microsoft Defender för Office 365 Valv för bifogade filer.</span><span class="sxs-lookup"><span data-stu-id="f217a-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="f217a-105">På så sätt undviker du meddelandefördröjningar och skyddar mottagarna från skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="f217a-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="f217a-106">**Vill du rapportera falska positiva eller falska negativa resultat till Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="f217a-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="f217a-107">Använd [Inskickade material i Utforskaren.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="f217a-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="f217a-108">-\*\* Visste du att du kan aktivera Valv för internt e-postmeddelande som skickas mellan mottagare inom din organisation?\*\* Följ de här stegen:</span><span class="sxs-lookup"><span data-stu-id="f217a-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="f217a-109">Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhetsadministratörskonto.</span><span class="sxs-lookup"><span data-stu-id="f217a-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="f217a-110">I det vänstra navigeringsfönstret under **Hothantering** väljer du **Valv** \> **Länkar**.</span><span class="sxs-lookup"><span data-stu-id="f217a-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="f217a-111">Markera **principen i avsnittet Principer som gäller för** hela organisationen och klicka på **Redigera.**</span><span class="sxs-lookup"><span data-stu-id="f217a-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="f217a-112">Under **Inställningar** aktiverar du **Använd säkra länkar för meddelanden som skickas inom organisationen.**</span><span class="sxs-lookup"><span data-stu-id="f217a-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
