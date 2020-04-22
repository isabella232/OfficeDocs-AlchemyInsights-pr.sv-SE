---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676515"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="6cf49-102">Åtgärda problem med e-postleverans för felkod 5.7.23</span><span class="sxs-lookup"><span data-stu-id="6cf49-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="6cf49-103">Verifiera SPF DNS-posten för din domän vid en allmänt tillgänglig SPF- eller DNS-inspelningskontroll på webben.</span><span class="sxs-lookup"><span data-stu-id="6cf49-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="6cf49-104">Kontrollera att det utgående meddelandet inte identifierades som skräppost av Microsoft och dirigerades via [högriskleveranspoolen](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="6cf49-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="6cf49-105">Meddelanden i högriskleveranspoolen klarar inte SPF-kontroller och accepteras därför inte av e-postorganisationen för målet.</span><span class="sxs-lookup"><span data-stu-id="6cf49-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="6cf49-106">Om problemet kvarstår kan du behöva kontakta administratören för den e-postvärd som du försöker skicka e-post till.</span><span class="sxs-lookup"><span data-stu-id="6cf49-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="6cf49-107">Anteckna det detaljerade externa felet i avvisningsmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="6cf49-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="6cf49-108">Microsoft-supporten kanske inte kan hjälpa till ytterligare.</span><span class="sxs-lookup"><span data-stu-id="6cf49-108">Microsoft support may not be able to assist further.</span></span>
