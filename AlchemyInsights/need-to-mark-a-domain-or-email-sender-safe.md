---
title: Behöver du markera en domän eller e-postavsändare som betrodd?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792150"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1e52c-102">Behöver du markera en domän eller e-postavsändare som betrodd?</span><span class="sxs-lookup"><span data-stu-id="1e52c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1e52c-103">Du bör **inte använda listor över betrodda** avsändare eftersom det öppnar organisationen för attacker av skräppost, phish och förfalskning.</span><span class="sxs-lookup"><span data-stu-id="1e52c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1e52c-104">Om det finns affärskrav rekommenderar vi emellertid att du **använder** **[e-postflödesregler för](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** detta.</span><span class="sxs-lookup"><span data-stu-id="1e52c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1e52c-105">Våra riktlinjer säkerställer att avsändarautentisering (verifierar att avsändarens domän inte kapas).</span><span class="sxs-lookup"><span data-stu-id="1e52c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1e52c-106">**Obs!** Vi rekommenderar inte att du hanterar falska positiva meddelanden med hjälp av listor över betrodda avsändare, eftersom undantag för skräppostfiltrering kan öppna organisationen för säkerhetsattacker.</span><span class="sxs-lookup"><span data-stu-id="1e52c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1e52c-107">Om användarna får meddelanden som felaktigt har markerats som skräppost ska du **[rapportera meddelanden och filer till Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="1e52c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1e52c-108">Betrodda avsändare i Outlook, lista över tillåtna avsändare  eller lista över tillåtna domäner i skydd mot skräppost bör undvikas eftersom avsändare kringgår all skräppost, förfalskningsskydd och säkerhets- och avsändarautentisering (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="1e52c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1e52c-109">Den här metoden används endast för temporär testning.</span><span class="sxs-lookup"><span data-stu-id="1e52c-109">This method is best used for temporary testing only.</span></span>
