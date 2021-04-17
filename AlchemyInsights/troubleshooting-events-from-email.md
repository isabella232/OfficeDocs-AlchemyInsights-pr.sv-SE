---
title: Felsökning av händelser från e-post
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834857"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="25649-102">Felsökning av händelser från e-post</span><span class="sxs-lookup"><span data-stu-id="25649-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="25649-103">Kontrollera att funktionen är aktiverad för postlådan: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="25649-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="25649-104">Titta sedan i loggarna "Händelser från **e-post" Exportera-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="25649-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="25649-105">I loggarna för händelser från e-post hittar du InternetMessageId som matchar objektet i postlådan.</span><span class="sxs-lookup"><span data-stu-id="25649-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="25649-106">TrustScore avgör om objektet läggs till eller inte.</span><span class="sxs-lookup"><span data-stu-id="25649-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="25649-107">Händelser läggs bara till om TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="25649-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="25649-108">TrustScore bestäms av egenskaperna SPF, Dkim eller Dmarc, som finns i meddelandehuvudet.</span><span class="sxs-lookup"><span data-stu-id="25649-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="25649-109">Så här visar du de här egenskaperna:</span><span class="sxs-lookup"><span data-stu-id="25649-109">To view these properties:</span></span>

<span data-ttu-id="25649-110">**Skrivbordsversionen av Outlook**</span><span class="sxs-lookup"><span data-stu-id="25649-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="25649-111">Öppna objektet</span><span class="sxs-lookup"><span data-stu-id="25649-111">Open the item</span></span>
- <span data-ttu-id="25649-112">Arkiv -> Egenskaper -> internethuvuden</span><span class="sxs-lookup"><span data-stu-id="25649-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="25649-113">eller</span><span class="sxs-lookup"><span data-stu-id="25649-113">or</span></span>

<span data-ttu-id="25649-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="25649-114">**MFCMapi**</span></span>

- <span data-ttu-id="25649-115">Navigera till objektet i Inkorgen</span><span class="sxs-lookup"><span data-stu-id="25649-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="25649-116">Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="25649-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="25649-117">Dessa egenskaper bestäms och registreras under transport och routning.</span><span class="sxs-lookup"><span data-stu-id="25649-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="25649-118">För ytterligare felsökning kan du behöva följa upp med TransportSupport om felen i SPF, DKIM och.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="25649-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>