---
title: Villkorad tillgång med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492662"
---
# <a name="conditional-access-with-intune"></a>Villkorad tillgång med Intune

**Villkorad tillgång** med Intune kräver 3 steg: 
  
- Skapa en **Princip för villkorlig åtkomst** som definierar vilka resurser skyddas och vad villkor måste uppfyllas för att få tillgång till dessa resurser. En enhet måste till exempel vara kompatibelt innan åtkomst till företagets e-post. 
    
- Skapa en **Princip för överensstämmelse** om du vill definiera inställningar som måste vara uppfyllda innan enheten anses vara kompatibla. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibla. 
    
- Att säkerställa både **Efterlevnad** och **Principer för villkorlig åtkomst** är riktade till önskad grupper av användare. Du kan behöva skapa specifika grupper av användare i Active Directory i Azure. 
    
Läs mer
  
- [Metodtips för villkorlig åtkomst](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [Komma igång med villkorad tillgång](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

