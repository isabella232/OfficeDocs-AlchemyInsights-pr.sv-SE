---
title: 2491 Varning e-postmeddelanden från "Phish Levereras på grund av klient eller användare åsidosätta" politik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758952"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="62518-102">Avisera e-postmeddelanden från principen "Phish Delivered på grund av klient- eller användaridosättning"</span><span class="sxs-lookup"><span data-stu-id="62518-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="62518-103">En standardaviseringsprincip med namnet "Phish Delivered på grund av klient- eller användar åsidosättning" har distribuerats till klienter med Office 365 ATP P1- och P2-licenser.</span><span class="sxs-lookup"><span data-stu-id="62518-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="62518-104">Om du har fått den här aviseringen är det här stegen för att undersöka:</span><span class="sxs-lookup"><span data-stu-id="62518-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="62518-105">Klicka på Visa **avisering** från **varningsmeddelandet** för att gå till sidan Aviseringar i säkerhets- & compliance center.</span><span class="sxs-lookup"><span data-stu-id="62518-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="62518-106">Markera aviseringen om du vill visa alternativet **Visa meddelandelista** eller **Visa meddelanden i Utforskaren**.</span><span class="sxs-lookup"><span data-stu-id="62518-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="62518-107">Båda dessa alternativ tar dig till informationen om meddelandet, som innehåller meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="62518-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="62518-108">Observera att länken Threat Explorer automatiskt filtrerar de meddelanden som matchar varningsvillkoren.</span><span class="sxs-lookup"><span data-stu-id="62518-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="62518-109">Du kan behöva justera datumfiltret i Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="62518-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="62518-110">Nätfiskemeddelandet levererades på grund av en manuellt konfigurerad åsidosättning:</span><span class="sxs-lookup"><span data-stu-id="62518-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="62518-111">En tillåten avsändare eller domän som angetts av användaren.</span><span class="sxs-lookup"><span data-stu-id="62518-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="62518-112">En tillåten avsändare eller domän som angetts av administratören i en policy mot skräppost.</span><span class="sxs-lookup"><span data-stu-id="62518-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="62518-113">En tillåten IP-adress i en anslutningsfilterprincip.</span><span class="sxs-lookup"><span data-stu-id="62518-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="62518-114">En regel för e-postflöde (kallas även en transportregel) som är konfigurerad för att tillåta meddelanden i.</span><span class="sxs-lookup"><span data-stu-id="62518-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="62518-115">Om du tror att meddelandet har markerats felaktigt som phish använder du [tillägget Outlook-rapportmeddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka meddelandeexempel till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="62518-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
