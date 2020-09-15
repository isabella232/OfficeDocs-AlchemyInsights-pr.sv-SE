---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717343"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="99c97-102">Korrigera problem med e-postleverans för felkod 5.7.23</span><span class="sxs-lookup"><span data-stu-id="99c97-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="99c97-103">Verifiera SPF DNS-posten för din domän hos en offentlig tillgänglig SPF-eller DNS-postkontroll på webben.</span><span class="sxs-lookup"><span data-stu-id="99c97-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="99c97-104">Kontrol lera att det utgående meddelandet inte identifierades som skräp post av Microsoft och dirigeras via [poolen med högrisk leveranser](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="99c97-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="99c97-105">Meddelanden i poolen med hög risk skickar inte SPF-kontroller och kommer därför inte att accepteras av mål-e-postorganisationen.</span><span class="sxs-lookup"><span data-stu-id="99c97-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="99c97-106">Om problemet kvarstår kan du behöva kontakta administratören hos e-postvärden som du försöker skicka e-post till.</span><span class="sxs-lookup"><span data-stu-id="99c97-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="99c97-107">Anteckna det detaljerade externa felet som är tillgängligt i studs meddelandet.</span><span class="sxs-lookup"><span data-stu-id="99c97-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="99c97-108">Microsoft Support kanske inte kan hjälpa till.</span><span class="sxs-lookup"><span data-stu-id="99c97-108">Microsoft support may not be able to assist further.</span></span>
