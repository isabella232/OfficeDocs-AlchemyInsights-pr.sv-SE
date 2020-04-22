---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710461"
---
# <a name="verify-your-domain"></a><span data-ttu-id="18d9f-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="18d9f-102">Verify your domain</span></span>

 <span data-ttu-id="18d9f-103">**Posten har förmodligen inte uppdaterats på Internet.**</span><span class="sxs-lookup"><span data-stu-id="18d9f-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="18d9f-104">Vanligtvis kan vi se den nya posten efter bara några minuter, men ibland kan det ta upp till några timmar.</span><span class="sxs-lookup"><span data-stu-id="18d9f-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="18d9f-105">Om du redan har väntat så länge dubbelkollar du att du har kopierat och klistrat in det exakta värdet i TXT-verifieringsposten hos din DNS-värd.</span><span class="sxs-lookup"><span data-stu-id="18d9f-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="18d9f-106">Ett vanligt problem är att man inte har tagit med "MS ="-delen av posten.</span><span class="sxs-lookup"><span data-stu-id="18d9f-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="18d9f-107">Vi behöver den också!</span><span class="sxs-lookup"><span data-stu-id="18d9f-107">We need that too!</span></span>

- <span data-ttu-id="18d9f-108">På vissa DNS-värdar måste du vidta extra åtgärd för att spara zonfilen (där DNS-posten lagras) så att den uppdateras på Internet.</span><span class="sxs-lookup"><span data-stu-id="18d9f-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="18d9f-109">Kontrollera att du har sparat ändringarna så att Microsoft kan se och verifiera posten.</span><span class="sxs-lookup"><span data-stu-id="18d9f-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
