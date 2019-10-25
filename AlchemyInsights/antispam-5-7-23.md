---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682316"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="13bcd-102">Åtgärda problem med e-postleverans för felkod 5.7.23</span><span class="sxs-lookup"><span data-stu-id="13bcd-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="13bcd-103">Kontrollera SPF DNS-posten för din domän på en offentligt tillgänglig SPF eller DNS-post Checker på webben.</span><span class="sxs-lookup"><span data-stu-id="13bcd-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="13bcd-104">Kontrollera att det utgående meddelandet inte identifierades som skräppost av Office 365 och dirigeras via [poolen med hög risk](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="13bcd-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="13bcd-105">Meddelanden i poolen med hög risk skickar inte SPF-kontroller och godkänns därför inte av destinations organisationen för e-post.</span><span class="sxs-lookup"><span data-stu-id="13bcd-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="13bcd-106">Om problemet kvarstår kan du behöva kontakta administratören för den e-postvärd som du försöker skicka e-post till.</span><span class="sxs-lookup"><span data-stu-id="13bcd-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="13bcd-107">Anteckna det detaljerade externa fel som finns i avvisningsmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="13bcd-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="13bcd-108">Support för Office 365 kanske inte kan hjälpa till ytterligare.</span><span class="sxs-lookup"><span data-stu-id="13bcd-108">Office 365 support may not be able to assist further.</span></span>