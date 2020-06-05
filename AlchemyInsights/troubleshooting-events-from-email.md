---
title: Felsöka händelser från e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569402"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4b888-102">Felsöka händelser från e-post</span><span class="sxs-lookup"><span data-stu-id="4b888-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4b888-103">Kontrollera att funktionen är aktiverad för postlådan: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="4b888-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4b888-104">Titta sedan på loggarna "Händelser från e-post" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4b888-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4b888-105">Leta reda på det InternetMessageId som matchar objektet i postlådan i loggarna "Händelser från e-post".</span><span class="sxs-lookup"><span data-stu-id="4b888-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4b888-106">TrustScore avgör om objektet läggs till eller inte.</span><span class="sxs-lookup"><span data-stu-id="4b888-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4b888-107">Händelser läggs bara till om TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="4b888-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4b888-108">TrustScore bestäms av SPF-, Dkim- eller Dmarc-egenskaper, som finns i meddelandehuvudet.</span><span class="sxs-lookup"><span data-stu-id="4b888-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4b888-109">Så här visar du dessa egenskaper:</span><span class="sxs-lookup"><span data-stu-id="4b888-109">To view these properties:</span></span>

<span data-ttu-id="4b888-110">**Outlook på skrivbordet**</span><span class="sxs-lookup"><span data-stu-id="4b888-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4b888-111">Öppna objektet</span><span class="sxs-lookup"><span data-stu-id="4b888-111">Open the item</span></span>
- <span data-ttu-id="4b888-112">Fil -> egenskaper -> Internet-huvuden</span><span class="sxs-lookup"><span data-stu-id="4b888-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4b888-113">eller</span><span class="sxs-lookup"><span data-stu-id="4b888-113">or</span></span>

<span data-ttu-id="4b888-114">**MFCMapi (på andra sätt)**</span><span class="sxs-lookup"><span data-stu-id="4b888-114">**MFCMapi**</span></span>

- <span data-ttu-id="4b888-115">Navigera till objektet i inkorgen</span><span class="sxs-lookup"><span data-stu-id="4b888-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4b888-116">Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4b888-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4b888-117">Dessa egenskaper bestäms och registreras under transport och routning.</span><span class="sxs-lookup"><span data-stu-id="4b888-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4b888-118">För ytterligare felsökning kan du behöva följa upp med Transport Support om felen i SPF, DKIM and.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="4b888-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>