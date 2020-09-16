---
title: Felsöka händelser från e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658752"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="a7850-102">Felsöka händelser från e-post</span><span class="sxs-lookup"><span data-stu-id="a7850-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="a7850-103">Kontrol lera att funktionen är aktive rad för post lådan: **get- <mailbox> EventsFromEmailConfiguration-Identity**</span><span class="sxs-lookup"><span data-stu-id="a7850-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="a7850-104">Titta sedan på "händelserna from E-mail"-loggarna **export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="a7850-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="a7850-105">Leta reda på InternetMessageId som matchar objektet i post lådan i loggarna händelser från e-post.</span><span class="sxs-lookup"><span data-stu-id="a7850-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="a7850-106">TrustScore bestämmer om objektet läggs till eller inte.</span><span class="sxs-lookup"><span data-stu-id="a7850-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="a7850-107">Händelser läggs endast till om TrustScore = "betrodd".</span><span class="sxs-lookup"><span data-stu-id="a7850-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="a7850-108">TrustScore bestäms av SPF-, DKIM-eller DMARC-egenskaper, som finns i meddelande huvudet.</span><span class="sxs-lookup"><span data-stu-id="a7850-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="a7850-109">Så här visar du dessa egenskaper:</span><span class="sxs-lookup"><span data-stu-id="a7850-109">To view these properties:</span></span>

<span data-ttu-id="a7850-110">**Outlook på Skriv bordet**</span><span class="sxs-lookup"><span data-stu-id="a7850-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="a7850-111">Öppna objektet</span><span class="sxs-lookup"><span data-stu-id="a7850-111">Open the item</span></span>
- <span data-ttu-id="a7850-112">Egenskaper för fil >-> Internet rubriker</span><span class="sxs-lookup"><span data-stu-id="a7850-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="a7850-113">eller</span><span class="sxs-lookup"><span data-stu-id="a7850-113">or</span></span>

<span data-ttu-id="a7850-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="a7850-114">**MFCMapi**</span></span>

- <span data-ttu-id="a7850-115">Navigera till objektet i Inkorgen</span><span class="sxs-lookup"><span data-stu-id="a7850-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="a7850-116">Leta efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="a7850-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="a7850-117">Dessa egenskaper bestäms och spelas in under transport och routning.</span><span class="sxs-lookup"><span data-stu-id="a7850-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="a7850-118">För ytterligare fel sökning kan du behöva följa upp transport stöd om felet i SPF-, DKIM-och. DMARC.</span><span class="sxs-lookup"><span data-stu-id="a7850-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>