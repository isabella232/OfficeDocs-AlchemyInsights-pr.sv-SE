---
title: 2491 Avisering e-postmeddelanden från principen "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544596"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="746a4-102">Avisering e-postmeddelanden från principen "Phish Delivered due to tenant or user override"</span><span class="sxs-lookup"><span data-stu-id="746a4-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="746a4-103">En standardaviseringsprincip med namnet "Phish Delivered due to tenant or user override" har distribuerats till klientorganisationen med Microsoft Defender för Office 365 P1- och P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="746a4-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="746a4-104">Om du fick det här aviseringen finns det anvisningar för att undersöka detta:</span><span class="sxs-lookup"><span data-stu-id="746a4-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="746a4-105">Från varningsmeddelandet klickar du **på Visa avisering** för **att** gå till sidan Aviseringar i & säkerhets- och efterlevnadscenter.</span><span class="sxs-lookup"><span data-stu-id="746a4-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="746a4-106">Välj aviseringen om du vill se alternativet **Visa meddelandelista eller** **Visa meddelanden i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="746a4-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="746a4-107">Båda dessa alternativ tar dig till meddelandets information, som innehåller Meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="746a4-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="746a4-108">Observera att länken Hotutforskaren automatiskt filtrerar meddelanden som matchar aviseringskriterierna.</span><span class="sxs-lookup"><span data-stu-id="746a4-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="746a4-109">Du kan behöva justera datumfiltret i Hotutforskaren.</span><span class="sxs-lookup"><span data-stu-id="746a4-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="746a4-110">Nätfiskemeddelandet levererades på grund av en manuellt konfigurerad åsidosättning:</span><span class="sxs-lookup"><span data-stu-id="746a4-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="746a4-111">En tillåten avsändare eller domän som har angetts av användaren.</span><span class="sxs-lookup"><span data-stu-id="746a4-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="746a4-112">En tillåten avsändare eller domän som anges av administratören i en princip mot skräppost.</span><span class="sxs-lookup"><span data-stu-id="746a4-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="746a4-113">En tillåten IP-adress i en princip för anslutningsfilter.</span><span class="sxs-lookup"><span data-stu-id="746a4-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="746a4-114">En e-postflödesregel (kallas även transportregel) som är konfigurerad för att tillåta meddelanden.</span><span class="sxs-lookup"><span data-stu-id="746a4-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="746a4-115">Om du anser att meddelandet felaktigt har markerats som phish använder du tillägget Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka exempel på meddelanden till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="746a4-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
