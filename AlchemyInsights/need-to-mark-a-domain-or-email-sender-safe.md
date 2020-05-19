---
title: Behöver du markera en domän eller e-postavsändare säker?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281189"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="46937-102">Behöver du markera en domän eller e-postavsändare säker?</span><span class="sxs-lookup"><span data-stu-id="46937-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="46937-103">Användning av **listor över betrodda avsändare rekommenderas inte** eftersom det öppnar organisationen för skräppost-, phish- och förfalskningsattacker.</span><span class="sxs-lookup"><span data-stu-id="46937-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="46937-104">Men om det finns ett affärskrav rekommenderar vi **att** du använder **[Mail Flow-regler](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** för detta.</span><span class="sxs-lookup"><span data-stu-id="46937-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="46937-105">Vår vägledning säkerställer att avsändarautentisering (verifierar att skicka domän inte förfalskas).</span><span class="sxs-lookup"><span data-stu-id="46937-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="46937-106">**Vi**rekommenderar inte att du hanterar falska positiva identifieringar med hjälp av säkra avsänningslistor, eftersom undantag från skräppostfiltrering kan öppna din organisation för säkerhetsattacker.</span><span class="sxs-lookup"><span data-stu-id="46937-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="46937-107">Om dina användare får meddelanden som felaktigt markerats som skräppost eller skräppost ska du **[rapportera meddelanden och filer till Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="46937-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="46937-108">Betrodda avsändare i Outlook, listan Överordnare eller tillåten domänlista i anti-spam-principer **bör undvikas** eftersom avsändare kringgår all skräppost, förfalskning och phish-skydd och avsändandeautentisering (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="46937-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="46937-109">Den här metoden används endast bäst för tillfälliga tester.</span><span class="sxs-lookup"><span data-stu-id="46937-109">This method is best used for temporary testing only.</span></span>
