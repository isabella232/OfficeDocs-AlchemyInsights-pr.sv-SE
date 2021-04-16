---
title: Frågor om hur du använder distributionsverktyget för Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790350"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Frågor om hur du använder distributionsverktyget för Office (ODT)

Ladda ned distributionsverktyget för Office från [Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
När du har laddat ned filen kör du den körbara filen som innehåller körbar fil (setup.exe) och en exempelkonfigurationsfil (configuration.xml).
  
 **Så här utesluter eller tar du bort Microsoft 365-appar för företag från klientdatorer:**
  
När du installerar Microsoft 365-appar för företag kan du utesluta specifika produkter. Det gör du genom att följa stegen för att installera Office med ODT,men ta med elementet ExcludeApp i konfigurationsfilen. Den här konfigurationsfilen installerar till exempel alla Microsoft 365-program för företagsprodukter förutom Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Översikt över distributionsverktyget för Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

