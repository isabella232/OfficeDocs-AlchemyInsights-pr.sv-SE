---
title: Frågor om hur du använder OFFICE Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698076"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Frågor om hur du använder OFFICE Deployment Tool (ODT)

Hämta distributionsverktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
När du har hämtat filen kör du den körbara filen som självextraherar, som innehåller office deployment tool-körbara (setup.exe) och en exempelkonfigurationsfil (configuration.xml).
  
 **Så här utesluter eller tar du bort Microsoft 365-appar för företagsprodukter från klientdatorer:**
  
När du installerar Microsoft 365 Apps för företag kan du utesluta specifika produkter. Det gör du genom att följa stegen för att installera Office med ODT, men inkludera excludeapp-elementet i konfigurationsfilen. Den här konfigurationsfilen installerar till exempel alla Microsoft 365-appar för företagsprodukter utom Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Översikt över distributionsverktyget för Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

