---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36505012"
---
# <a name="conditional-access-with-intune"></a>Villkorlig åtkomst med Intune

Med **villkorlig åtkomst** med Intune krävs 3 steg: 
  
- Skapa en **princip för villkorlig åtkomst** som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser. Till exempel måste en enhet vara kompatibel innan du får tillgång till företagets e-post. 
    
- Skapa en **efterlevnadsprincip** för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel. En enhet måste till exempel ha en PIN-kod på minst 6 siffror innan den anses vara kompatibel. 
    
- Se till att både **efterlevnadsprinciper** och **principer för villkorlig åtkomst** är riktade till önskade grupper av användare. Detta kan kräva att skapa specifika grupper av användare i Azure Active Directory. 
    
Läs mer:
  
- [Metodtips för villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Komma igång med villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

