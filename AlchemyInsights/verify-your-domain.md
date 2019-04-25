---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d215f3af0cf4b46b12c8cb51a9572adb00f354e4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420070"
---
# <a name="verify-your-domain"></a><span data-ttu-id="cdc5a-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="cdc5a-102">Verify your domain</span></span>

 <span data-ttu-id="cdc5a-103">**Förmodligen uppdatera inte posten via Internet.**</span><span class="sxs-lookup"><span data-stu-id="cdc5a-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="cdc5a-104">Vanligtvis kan vi se den nya posten efter bara några minuter, men ibland kan det ta upp till några timmar.</span><span class="sxs-lookup"><span data-stu-id="cdc5a-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="cdc5a-105">Om du har väntat som redan länge dubbelkolla att du har kopieras och klistras in det exakta värdet i kontrollen TXT-posten i din DNS-värd.</span><span class="sxs-lookup"><span data-stu-id="cdc5a-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="cdc5a-106">Ett vanligt problem är att man inte har tagit med "MS ="-delen av posten.</span><span class="sxs-lookup"><span data-stu-id="cdc5a-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="cdc5a-107">Vi behöver den också!</span><span class="sxs-lookup"><span data-stu-id="cdc5a-107">We need that too!</span></span>
    
- <span data-ttu-id="cdc5a-108">På vissa DNS-värdar måste du vidta extra åtgärd för att spara zonfilen (där DNS-posten lagras) så att den uppdateras på Internet.</span><span class="sxs-lookup"><span data-stu-id="cdc5a-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="cdc5a-109">Kontrollera att du har sparat ändringarna så att Office 365 kan se och verifiera posten.</span><span class="sxs-lookup"><span data-stu-id="cdc5a-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

