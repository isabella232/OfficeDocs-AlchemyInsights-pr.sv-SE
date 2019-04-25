---
title: Frågor om hur du använder Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371786"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Frågor om hur du använder Office Deployment Tool (ODT)

Hämta Office Deployment Tool på [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
När du har hämtat filen att köra den självextraherande körbara filen som innehåller Office Deployment Tool körbara (setup.exe) och exempel konfigurationsfil (configuration.xml).
  
 **Utesluta eller ta bort Office 365 ProPlus produkter från klientdatorer:**
  
När du installerar Office 365 ProPlus, kan du utesluta specifika produkter. Följ instruktionerna för att installera Office med ODT gör, men inkludera elementet ExcludeApp i konfigurationsfilen. Till exempel installerar konfigurationsfilen Office 365 ProPlus produkter utom Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Översikt över Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

