---
title: Konvertering av postlåda till en delad postlåda?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496453"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="cbc48-102">Konvertera en postlåda för användaren till en delad postlåda</span><span class="sxs-lookup"><span data-stu-id="cbc48-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="cbc48-103">Du kan bara konvertera en postlåda till en delad postlåda om användaren har en Exchange-licens.</span><span class="sxs-lookup"><span data-stu-id="cbc48-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="cbc48-104">När postlådan har konverterats, fortsätter den att visas i användarlistan över aktiva eftersom listan innehåller delade postlådor.</span><span class="sxs-lookup"><span data-stu-id="cbc48-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="cbc48-105">Men visas den konverterade postlådan också i listan över delade postlådor.</span><span class="sxs-lookup"><span data-stu-id="cbc48-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="cbc48-106">Om du försöker konvertera en postlåda i Exchange Admin Console och konverteringen misslyckas, rensa din webbläsarens cacheminne och cookies och försök igen.</span><span class="sxs-lookup"><span data-stu-id="cbc48-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="cbc48-107">Om det fortfarande inte fungerar kan du försöka konvertera postlåda i Exchange Management Shell genom att köra följande kommando:</span><span class="sxs-lookup"><span data-stu-id="cbc48-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="cbc48-108">Mer information om postlåda finns i [Konvertera en postlåda till en delad postlåda](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="cbc48-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
