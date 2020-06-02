---
title: Felsöka avancerat hotskydd för Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512608"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="0504f-102">Felsöka avancerat hotskydd för Office 365</span><span class="sxs-lookup"><span data-stu-id="0504f-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="0504f-103">Märker du förseningar i meddelandeleveransen?</span><span class="sxs-lookup"><span data-stu-id="0504f-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="0504f-104">Använd alternativet [Dynamisk leverans](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i atp-principen för säkra bilagor.</span><span class="sxs-lookup"><span data-stu-id="0504f-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="0504f-105">Detta hjälper till att undvika meddelandefördröjningar samtidigt som mottagare skyddas från skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="0504f-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="0504f-106">Vill du rapportera falska positiva eller falska negativ till Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0504f-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="0504f-107">Använd den här [länken](https://www.microsoft.com/wdsi/filesubmission/) för att skicka filer för analys.</span><span class="sxs-lookup"><span data-stu-id="0504f-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="0504f-108">Visste du att du kan aktivera skydd för säkra länkar för intern e-post som skickas mellan mottagare inom organisationen?</span><span class="sxs-lookup"><span data-stu-id="0504f-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="0504f-109">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="0504f-109">Follow these steps:</span></span>

  1. <span data-ttu-id="0504f-110">Gå till [https://protection.office.com](https://protection.office.com) och logga in med ett globalt administratörs- eller säkerhetsadministratörskonto.</span><span class="sxs-lookup"><span data-stu-id="0504f-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="0504f-111">Välj **Säkra principlänkar** i det vänstra navigeringsfönstret under **Hothantering** \> **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="0504f-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="0504f-112">Markera principen i avsnittet **Principer som gäller för hela organisationen** och klicka på **Redigera**.</span><span class="sxs-lookup"><span data-stu-id="0504f-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="0504f-113">Aktivera Tillämpa **säkra länkar på meddelanden som skickas inom organisationen**under **Inställningar**.</span><span class="sxs-lookup"><span data-stu-id="0504f-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
