---
title: Frågor om hur du använder distributions verktyget för Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086174"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Frågor om hur du använder distributions verktyget för Office (ODT)

Ladda ned distributions verktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
När du har laddat ned filen kör du den självextraherande körbara filen som innehåller installations programmet för Office (setupodt.exe) och en exempel konfigurations fil (configuration.xml).
  
 **Så här undantar eller tar du bort Microsoft 365-appar för företags produkter från klient datorer:**
  
När du installerar Microsoft 365-appar för företag kan du exkludera vissa produkter. Om du vill göra det följer du anvisningarna för att installera Office med ODT, men inkluderar elementet ExcludeApp i konfigurations filen. Med den här konfigurations filen installeras till exempel alla Microsoft 365-appar för företags produkter förutom Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Översikt över distributions verktyget för Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

