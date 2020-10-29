---
title: Felsöka Microsoft Defender för Office 365
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801464"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="43150-102">Felsöka Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="43150-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="43150-103">Märker du fördröjningar i leverans av meddelanden?</span><span class="sxs-lookup"><span data-stu-id="43150-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="43150-104">Använd alternativet [dynamisk leverans](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i policyn för säker användning för ATP.</span><span class="sxs-lookup"><span data-stu-id="43150-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="43150-105">Detta hjälper till att undvika meddelande fördröjningar när du skyddar mottagare från skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="43150-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="43150-106">Vill du rapportera falsk positiv eller falsk negativ till Microsoft?</span><span class="sxs-lookup"><span data-stu-id="43150-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="43150-107">Använd den här [länken](https://www.microsoft.com/wdsi/filesubmission/) om du vill skicka filer för analys.</span><span class="sxs-lookup"><span data-stu-id="43150-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="43150-108">Visste du att du kan aktivera skydd mot säkra Länkar för intern e-post som skickas mellan mottagarna inom din organisation?</span><span class="sxs-lookup"><span data-stu-id="43150-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="43150-109">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="43150-109">Follow these steps:</span></span>

  1. <span data-ttu-id="43150-110">Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhets administratörs konto.</span><span class="sxs-lookup"><span data-stu-id="43150-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="43150-111">Välj **policy** Safe Links i det vänstra navigerings fönstret under **Threat Management** \> **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="43150-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="43150-112">I de **principer som gäller för hela avsnittet organisation** väljer du policy och klickar på **Redigera** .</span><span class="sxs-lookup"><span data-stu-id="43150-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="43150-113">Under **Inställningar** aktiverar **du Använd Safe Links för meddelanden som skickas inom organisationen** .</span><span class="sxs-lookup"><span data-stu-id="43150-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
