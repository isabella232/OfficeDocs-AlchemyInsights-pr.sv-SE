---
title: Skydd motspam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821429"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="d7d44-102">Korrigera problem med e-postleverans för felkod 5.7.23</span><span class="sxs-lookup"><span data-stu-id="d7d44-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="d7d44-103">Verifiera SPF DNS-posten för din domän på en offentligt tillgänglig SPF- eller DNS-postkontroll på webben.</span><span class="sxs-lookup"><span data-stu-id="d7d44-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="d7d44-104">Kontrollera att det utgående meddelandet inte identifierats som skräppost av Microsoft och dirigerats via [Högriskleveranspool.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="d7d44-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="d7d44-105">Meddelanden i högriskleveranspoolen passerar inte SPF-kontroller och accepteras därför inte av mål-e-postorganisationen.</span><span class="sxs-lookup"><span data-stu-id="d7d44-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="d7d44-106">Om problemet kvarstår kan du behöva kontakta administratören för e-postvärden som du försöker skicka e-post till.</span><span class="sxs-lookup"><span data-stu-id="d7d44-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="d7d44-107">Anteckna det detaljerade externa felet som finns i studsande meddelandet.</span><span class="sxs-lookup"><span data-stu-id="d7d44-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="d7d44-108">Microsoft Support kanske inte kan hjälpa dig vidare.</span><span class="sxs-lookup"><span data-stu-id="d7d44-108">Microsoft support may not be able to assist further.</span></span>
