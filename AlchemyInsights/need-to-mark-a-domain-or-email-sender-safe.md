---
title: Behöver du markera en domän eller e-post avsändare?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803263"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="0b72d-102">Behöver du markera en domän eller e-post avsändare?</span><span class="sxs-lookup"><span data-stu-id="0b72d-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="0b72d-103">Användning av **listor för säkra avsändare rekommenderas inte** eftersom den öppnar din organisation för skräp post, Phish och förfalskningar.</span><span class="sxs-lookup"><span data-stu-id="0b72d-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="0b72d-104">Om det finns ett företags behov **rekommenderar** vi att du använder **[regler för e-postflöde](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** för detta.</span><span class="sxs-lookup"><span data-stu-id="0b72d-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="0b72d-105">Vår vägledning säkerställer att avsändaren (verifierar att sändande domän inte är falsk).</span><span class="sxs-lookup"><span data-stu-id="0b72d-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="0b72d-106">**Obs!** vi rekommenderar inte att du hanterar falsk identifiering genom att använda listor med säkra avsändare, eftersom undantag för skräp post filtrering kan öppna din organisation för säkerhets attacker.</span><span class="sxs-lookup"><span data-stu-id="0b72d-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="0b72d-107">Om dina användare (er) får meddelanden som är felaktigt markerade som skräp post, kan du **[rapportera meddelanden och filer till Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="0b72d-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="0b72d-108">Betrodda avsändare i Outlook, listan med tillåtna avsändare eller tillåtna domäner i principer för skräp post skydd **bör undvikas** eftersom avsändare kringgår all skräp post, falsk identitet och phishskydd (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="0b72d-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="0b72d-109">Den här metoden är bäst för tillfälliga tester.</span><span class="sxs-lookup"><span data-stu-id="0b72d-109">This method is best used for temporary testing only.</span></span>
