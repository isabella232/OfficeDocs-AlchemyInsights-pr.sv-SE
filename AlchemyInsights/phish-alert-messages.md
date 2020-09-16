---
title: 2491 Avisera e-postmeddelanden från principen "Phish som skickas på grund av klient-eller användar åsidosättningar"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728629"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="14e57-102">Avisera e-postmeddelanden från principen "Phish som skickas på grund av klient-eller användar åsidosättningar"</span><span class="sxs-lookup"><span data-stu-id="14e57-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="14e57-103">En standard aviserings princip med namnet "Phish levererad på grund av klient-eller användar åsidosättning" har distribuerats till klient organisationer med Office 365 ATP-och P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="14e57-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="14e57-104">Om du fick den här aviseringen kan du undersöka:</span><span class="sxs-lookup"><span data-stu-id="14e57-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="14e57-105">Klicka på **Visa varning** i aviserings meddelandet för att gå till sidan **aviseringar** i säkerhets & efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="14e57-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="14e57-106">Välj varningen om du vill se alternativet att **Visa meddelande listan** eller **Visa meddelanden i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="14e57-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="14e57-107">Båda dessa alternativ tar dig till meddelandets information, som innehåller meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="14e57-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="14e57-108">Observera att länken Threat Explorer automatiskt filtrerar meddelanden som matchar aviserings villkoren.</span><span class="sxs-lookup"><span data-stu-id="14e57-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="14e57-109">Du kan behöva justera datum filtret i Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="14e57-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="14e57-110">Nät fiske meddelandet levererades på grund av en manuellt konfigurerad åsidosättning:</span><span class="sxs-lookup"><span data-stu-id="14e57-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="14e57-111">En avsändare eller domän som anges av användaren.</span><span class="sxs-lookup"><span data-stu-id="14e57-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="14e57-112">En avsändare eller domän som angetts av administratören i en policy för skräp post.</span><span class="sxs-lookup"><span data-stu-id="14e57-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="14e57-113">En tillåten IP-adress i en anslutnings filter princip.</span><span class="sxs-lookup"><span data-stu-id="14e57-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="14e57-114">En regel för e-postflöde (kallas även transport regel) som är konfigurerad för att tillåta meddelanden i.</span><span class="sxs-lookup"><span data-stu-id="14e57-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="14e57-115">Om du tror att meddelandet inte hade marker ATS som Phish kan du använda [tillägget Outlook rapportera meddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka meddelanden till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="14e57-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
