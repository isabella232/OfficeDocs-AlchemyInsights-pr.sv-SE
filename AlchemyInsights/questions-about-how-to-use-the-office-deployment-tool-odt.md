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
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553558"
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
  

