---
title: 2491 alert e-postmeddelanden från Phish levereras innehavare eller användare åsidosätter principen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391564"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="ebf88-102">Alert e-postmeddelanden från Phish levereras innehavare eller användare åsidosätter principen</span><span class="sxs-lookup"><span data-stu-id="ebf88-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="ebf88-103">En varning standardprincipen ”Phish levererad på Åsidosätt innehavare eller användare” har ångrats till hyresgäster med licenser för Office 365 ATP P1 och P2.</span><span class="sxs-lookup"><span data-stu-id="ebf88-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="ebf88-104">Här är stegen för att undersöka om du fått denna varning:</span><span class="sxs-lookup"><span data-stu-id="ebf88-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="ebf88-105">Meddelande, klicka på **Visa varning** att gå till sidan **meddelanden** i säkerhet & regelefterlevnadscentret.</span><span class="sxs-lookup"><span data-stu-id="ebf88-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="ebf88-106">Markera aviseringen till finns alternativ för att **Visa meddelandelista** eller **Visa meddelanden i Explorer**.</span><span class="sxs-lookup"><span data-stu-id="ebf88-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="ebf88-107">Båda dessa alternativ om du vill ha information om meddelandet, som innehåller meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="ebf88-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="ebf88-108">Observera att länken hot Explorer automatiskt ska filtrera meddelanden som matchar aviseringsvillkoren.</span><span class="sxs-lookup"><span data-stu-id="ebf88-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="ebf88-109">Du kan behöva justera Datumfilter i Explorer hot.</span><span class="sxs-lookup"><span data-stu-id="ebf88-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="ebf88-110">Phishing-meddelandet levererades på grund av en manuellt konfigurerad åsidosättning:</span><span class="sxs-lookup"><span data-stu-id="ebf88-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="ebf88-111">En tillåtna avsändare eller domän som anges av användaren.</span><span class="sxs-lookup"><span data-stu-id="ebf88-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="ebf88-112">En tillåtna avsändare eller domän som anges av admin i en policy mot skräppost.</span><span class="sxs-lookup"><span data-stu-id="ebf88-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="ebf88-113">En tillåtna IP-adress i en princip för filtret.</span><span class="sxs-lookup"><span data-stu-id="ebf88-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="ebf88-114">E-post flöde regel (kallas även en transportregel) som är konfigurerad för att tillåta meddelanden i.</span><span class="sxs-lookup"><span data-stu-id="ebf88-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="ebf88-115">Om du tror att meddelandet var felaktigt markerad som nätfiske, använda Outlook [tillägget rapportmeddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att överlämna prover av meddelande till Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ebf88-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
