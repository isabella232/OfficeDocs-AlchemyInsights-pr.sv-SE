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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="664dd-102">Frågor om hur du använder distributionsverktyget för Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="664dd-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="664dd-103">Ladda ned distributionsverktyget för Office från [Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="664dd-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="664dd-104">När du har laddat ned filen kör du den körbara filen som innehåller körbar fil (setup.exe) och en exempelkonfigurationsfil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="664dd-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="664dd-105">**Så här utesluter eller tar du bort Microsoft 365-appar för företag från klientdatorer:**</span><span class="sxs-lookup"><span data-stu-id="664dd-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="664dd-106">När du installerar Microsoft 365-appar för företag kan du utesluta specifika produkter.</span><span class="sxs-lookup"><span data-stu-id="664dd-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="664dd-107">Det gör du genom att följa stegen för att installera Office med ODT,men ta med elementet ExcludeApp i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="664dd-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="664dd-108">Den här konfigurationsfilen installerar till exempel alla Microsoft 365-program för företagsprodukter förutom Publisher:</span><span class="sxs-lookup"><span data-stu-id="664dd-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="664dd-109">Översikt över distributionsverktyget för Office</span><span class="sxs-lookup"><span data-stu-id="664dd-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

