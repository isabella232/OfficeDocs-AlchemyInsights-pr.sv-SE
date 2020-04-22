---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706039"
---
# <a name="conditional-access-with-intune"></a>Villkorlig åtkomst med Intune

Om du använder **villkorlig åtkomst** med Intune krävs 3 steg: 
  
- Skapa en **princip för villkorlig åtkomst** som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser. En enhet måste till exempel vara kompatibel innan den får åtkomst till företagets e-post. 
    
- Skapa en **efterlevnadsprincip** för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel. En enhet måste till exempel ha en stift på minst 6 siffror innan den anses vara kompatibel. 
    
- Se till att både **efterlevnadsprinciper** och **principer för villkorlig åtkomst** är inriktade på önskade användargrupper. Detta kan kräva att du skapar specifika grupper av användare i Azure Active Directory. 
    
Läs mer:
  
- [Metodtips för villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Komma igång med villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

