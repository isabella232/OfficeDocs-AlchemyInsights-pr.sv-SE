---
title: Villkorad tillgång med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393559"
---
# <a name="conditional-access-with-intune"></a>Villkorad tillgång med Intune

**Villkorad tillgång** med Intune kräver 3 steg: 
  
- Skapa en **Princip för villkorlig åtkomst** som definierar vilka resurser skyddas och vad villkor måste uppfyllas för att få tillgång till dessa resurser. En enhet måste till exempel vara kompatibelt innan åtkomst till företagets e-post. 
    
- Skapa en **Princip för överensstämmelse** om du vill definiera inställningar som måste vara uppfyllda innan enheten anses vara kompatibla. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibla. 
    
- Att säkerställa både **Efterlevnad** och **Principer för villkorlig åtkomst** är riktade till önskad grupper av användare. Du kan behöva skapa specifika grupper av användare i Active Directory i Azure. 
    
Läs mer:
  
- [Metodtips för villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Komma igång med villkorad tillgång](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

