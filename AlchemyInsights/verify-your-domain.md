---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771009"
---
# <a name="verify-your-domain"></a><span data-ttu-id="eb532-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="eb532-102">Verify your domain</span></span>

 <span data-ttu-id="eb532-103">**Posten har förmodligen inte uppdaterats på Internet.**</span><span class="sxs-lookup"><span data-stu-id="eb532-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="eb532-104">Vanligtvis kan vi se den nya posten efter bara några minuter, men ibland kan det ta upp till några timmar.</span><span class="sxs-lookup"><span data-stu-id="eb532-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="eb532-105">Om du redan har väntat så länge kontrollerar du att du har kopierat och klistrat in det exakta värdet i TXT-verifieringsposten hos din DNS-värd.</span><span class="sxs-lookup"><span data-stu-id="eb532-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="eb532-106">Ett vanligt problem är att man inte har tagit med "MS ="-delen av posten.</span><span class="sxs-lookup"><span data-stu-id="eb532-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="eb532-107">Vi behöver den också!</span><span class="sxs-lookup"><span data-stu-id="eb532-107">We need that too!</span></span>

- <span data-ttu-id="eb532-108">På vissa DNS-värdar måste du vidta extra åtgärd för att spara zonfilen (där DNS-posten lagras) så att den uppdateras på Internet.</span><span class="sxs-lookup"><span data-stu-id="eb532-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="eb532-109">Kontrollera att du har sparat ändringarna så att Microsoft kan se och verifiera posten.</span><span class="sxs-lookup"><span data-stu-id="eb532-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
