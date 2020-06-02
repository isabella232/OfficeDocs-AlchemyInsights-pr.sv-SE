---
title: Felsöka problem med Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511130"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="a6017-102">Felsöka problem med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="a6017-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="a6017-103">**Märker förseningar med e-postleverans?**</span><span class="sxs-lookup"><span data-stu-id="a6017-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="a6017-104">Prova att använda alternativet Dynamisk leverans för dina ATP-principer för säkra bilagor.</span><span class="sxs-lookup"><span data-stu-id="a6017-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="a6017-105">På så sätt undviker du förseningar i leveransen av e-postmeddelanden samtidigt som mottagare skyddas från skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="a6017-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="a6017-106">**Vill du rapportera falska positiva eller falska negativ?**</span><span class="sxs-lookup"><span data-stu-id="a6017-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="a6017-107">Använd den här länken för att skicka in filen för analys:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="a6017-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="a6017-108">**Visste du att du kan aktivera ATP Safe Links skydd för e-post som skickas mellan personer i din organisation?**</span><span class="sxs-lookup"><span data-stu-id="a6017-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="a6017-109">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="a6017-109">Follow these steps:</span></span>
    1. <span data-ttu-id="a6017-110">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="a6017-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="a6017-111">Gå till säkra länkar **för**  >  **Policy**  >  **hothanteringspolicy .**</span><span class="sxs-lookup"><span data-stu-id="a6017-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="a6017-112">Redigera (eller lägga till) en princip under **Principer som gäller för specifika mottagare.**</span><span class="sxs-lookup"><span data-stu-id="a6017-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="a6017-113">Välj **Använd säkra länkar till meddelanden som skickas inom organisationen**.</span><span class="sxs-lookup"><span data-stu-id="a6017-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="a6017-114">Spara din princip och tillåt cirka 30 minuter för dina ändringar att arbeta sig igenom ditt datacenter.</span><span class="sxs-lookup"><span data-stu-id="a6017-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="a6017-115">Mer hjälp med ATP finns i [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="a6017-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>