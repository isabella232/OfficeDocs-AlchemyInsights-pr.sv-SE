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
Du kan bara konvertera en postlåda till en delad postlåda om användaren har en Exchange-licens. När postlådan har konverterats, fortsätter den att visas i användarlistan över aktiva eftersom listan innehåller delade postlådor. Men visas den konverterade postlådan också i listan över delade postlådor. 
  
Om du försöker konvertera en postlåda i Exchange Admin Console och konverteringen misslyckas, rensa din webbläsarens cacheminne och cookies och försök igen. Om det fortfarande inte fungerar kan du försöka konvertera postlåda i Exchange Management Shell genom att köra följande kommando:
  
```
Set-Mailbox -Type Shared
```

Mer information om postlåda finns i [Konvertera en postlåda till en delad postlåda](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
