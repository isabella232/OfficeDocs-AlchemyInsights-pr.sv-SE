---
title: Konvertering av postlåda till en delad postlåda?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492088"
---
<span data-ttu-id="30067-p101">Du kan bara konvertera en postlåda till en delad postlåda om användaren har en Exchange-licens. När postlådan har konverterats, fortsätter den att visas i användarlistan över aktiva eftersom listan innehåller delade postlådor. Men visas den konverterade postlådan också i listan över delade postlådor.</span><span class="sxs-lookup"><span data-stu-id="30067-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="30067-p102">Om du försöker konvertera en postlåda i Exchange Admin Console och konverteringen misslyckas, rensa din webbläsarens cacheminne och cookies och försök igen. Om det fortfarande inte fungerar kan du försöka konvertera postlåda i Exchange Management Shell genom att köra följande kommando:</span><span class="sxs-lookup"><span data-stu-id="30067-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="30067-107">Mer information om postlåda finns i [Konvertera en postlåda till en delad postlåda](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="30067-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
