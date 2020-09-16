---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734324"
---
# <a name="verify-your-domain"></a><span data-ttu-id="b9b69-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="b9b69-102">Verify your domain</span></span>

 <span data-ttu-id="b9b69-103">**Posten har antagligen inte uppdaterats på Internet.**</span><span class="sxs-lookup"><span data-stu-id="b9b69-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="b9b69-104">Vanligtvis kan vi se den nya posten efter bara några minuter, men ibland kan det ta upp till några timmar.</span><span class="sxs-lookup"><span data-stu-id="b9b69-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="b9b69-105">Om du har väntat att det är långt, kontrollerar du att du har kopierat och klistrat in det exakta värdet i TXT-verifierings posten hos DNS-värden.</span><span class="sxs-lookup"><span data-stu-id="b9b69-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="b9b69-106">Ett vanligt problem är att man inte har tagit med "MS ="-delen av posten.</span><span class="sxs-lookup"><span data-stu-id="b9b69-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="b9b69-107">Vi behöver den också!</span><span class="sxs-lookup"><span data-stu-id="b9b69-107">We need that too!</span></span>

- <span data-ttu-id="b9b69-108">På vissa DNS-värdar måste du vidta extra åtgärd för att spara zonfilen (där DNS-posten lagras) så att den uppdateras på Internet.</span><span class="sxs-lookup"><span data-stu-id="b9b69-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="b9b69-109">Kontrol lera att du har sparat ändringarna så att Microsoft kan se och bekräfta posten.</span><span class="sxs-lookup"><span data-stu-id="b9b69-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
