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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konvertera en postlåda för användaren till en delad postlåda

Du kan bara konvertera en postlåda till en delad postlåda om användaren har en Exchange-licens. När postlådan har konverterats, fortsätter den att visas i användarlistan över aktiva eftersom listan innehåller delade postlådor. Men visas den konverterade postlådan också i listan över delade postlådor. 
  
Om du försöker konvertera en postlåda i Exchange Admin Console och konverteringen misslyckas, rensa din webbläsarens cacheminne och cookies och försök igen. Om det fortfarande inte fungerar kan du försöka konvertera postlåda i Exchange Management Shell genom att köra följande kommando:
  
```
Set-Mailbox -Type Shared
```

Mer information om postlåda finns i [Konvertera en postlåda till en delad postlåda](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
