---
title: Felsöka problem med Microsoft Defender för Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801425"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="d71c1-102">Felsöka problem med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="d71c1-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="d71c1-103">**Har du några fördröjningar när du skickar e-** postmeddelanden?</span><span class="sxs-lookup"><span data-stu-id="d71c1-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="d71c1-104">Prova att använda alternativet dynamisk leverans för dina principer för säker användning av ATP.</span><span class="sxs-lookup"><span data-stu-id="d71c1-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="d71c1-105">Detta eliminerar fördröjning i e-postmeddelande när mottagare skyddas från skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="d71c1-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="d71c1-106">**Vill du rapportera falsk positiv eller falskt negativ** ?</span><span class="sxs-lookup"><span data-stu-id="d71c1-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="d71c1-107">Använd den här länken för att skicka filen för analys: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="d71c1-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="d71c1-108">**Visste du att du kan aktivera säkerhet för säkerhet för ATP för e-post som skickas mellan personer i organisationen** ?</span><span class="sxs-lookup"><span data-stu-id="d71c1-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="d71c1-109">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="d71c1-109">Follow these steps:</span></span>
    1. <span data-ttu-id="d71c1-110">Gå till https://protection.office.com och logga in.</span><span class="sxs-lookup"><span data-stu-id="d71c1-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="d71c1-111">Gå till säkra Länkar för **hot Management**  >  **policy**  >  **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="d71c1-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="d71c1-112">Redigera (eller Lägg till) en princip under **principer som gäller för specifika mottagare** .</span><span class="sxs-lookup"><span data-stu-id="d71c1-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="d71c1-113">Välj **Använd Safe Links för meddelanden som skickas inom organisationen** .</span><span class="sxs-lookup"><span data-stu-id="d71c1-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="d71c1-114">Spara policyn och låt ca 30 minuter för dina ändringar att fungera via ditt data Center.</span><span class="sxs-lookup"><span data-stu-id="d71c1-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="d71c1-115">Om du vill ha mer hjälp med ATP läser du [Microsoft Defender för Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="d71c1-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>