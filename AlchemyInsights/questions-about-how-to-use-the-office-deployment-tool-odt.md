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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553558"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="7514e-102">Frågor om hur du använder Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="7514e-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="7514e-103">Hämta Office Deployment Tool från [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="7514e-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="7514e-104">När du har hämtat filen kör du den självextraherande körbara filen, som innehåller det körbara programmet för Office Deployment Tool (Setup. exe) och en exempelkonfigurationsfil (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="7514e-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="7514e-105">**Så här utesluter eller tar du bort Office 365 ProPlus-produkter från klientdatorer:**</span><span class="sxs-lookup"><span data-stu-id="7514e-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="7514e-106">När du installerar Office 365 ProPlus kan du utesluta vissa produkter.</span><span class="sxs-lookup"><span data-stu-id="7514e-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="7514e-107">Om du vill göra det följer du stegen för att installera Office med ODT, men inkludera den ExcludeApp elementet i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="7514e-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="7514e-108">Den här konfigurationsfilen installerar till exempel alla Office 365 ProPlus-produkter utom Publisher:</span><span class="sxs-lookup"><span data-stu-id="7514e-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="7514e-109">Översikt över Office Deployment Tool</span><span class="sxs-lookup"><span data-stu-id="7514e-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

