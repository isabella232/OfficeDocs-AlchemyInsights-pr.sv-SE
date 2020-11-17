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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="e6b41-102">Frågor om hur du använder distributions verktyget för Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="e6b41-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e6b41-103">Ladda ned distributions verktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="e6b41-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="e6b41-104">När du har laddat ned filen kör du den självextraherande körbara filen som innehåller installations programmet för Office (setupodt.exe) och en exempel konfigurations fil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="e6b41-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="e6b41-105">**Så här undantar eller tar du bort Microsoft 365-appar för företags produkter från klient datorer:**</span><span class="sxs-lookup"><span data-stu-id="e6b41-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="e6b41-106">När du installerar Microsoft 365-appar för företag kan du exkludera vissa produkter.</span><span class="sxs-lookup"><span data-stu-id="e6b41-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="e6b41-107">Om du vill göra det följer du anvisningarna för att installera Office med ODT, men inkluderar elementet ExcludeApp i konfigurations filen.</span><span class="sxs-lookup"><span data-stu-id="e6b41-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="e6b41-108">Med den här konfigurations filen installeras till exempel alla Microsoft 365-appar för företags produkter förutom Publisher:</span><span class="sxs-lookup"><span data-stu-id="e6b41-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="e6b41-109">Översikt över distributions verktyget för Office</span><span class="sxs-lookup"><span data-stu-id="e6b41-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

