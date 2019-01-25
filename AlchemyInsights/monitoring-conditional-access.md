---
title: Övervakning av villkorad tillgång
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491835"
---
# <a name="monitoring-conditional-access"></a>Övervakning av villkorad tillgång

Riktade med villkorad tillgång användare får ett e-postmeddelanden om de inte uppfyller kraven i din organisation åtkomst. Lös, rekommenderar vi en eller flera av följande lösningar:
  
- Om enheten antas vara anmäld, informera användaren att gå till appen företagsportal och kontrollera att det visas i företagets Portal. Användaren bör registrera enheten om den inte.
    
- Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **enheten överensstämmelse**under **Bildskärm** . Visa enheten överensstämmelse rapporten för att kontrollera att användarens enhet är markerad som kompatibla. 
    
- Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **principer**under **Hantera**. I listan över principer för att kontrollera att en profil har tilldelats användarens enhet. Om ingen profil tilldelas Intune inte bekräfta överensstämmelse Enhetsstatus. 
    
- Redigera Användartilldelning villkorad tillgång.
    
1. Gå till Azure portal **Intune \> villkorad tillgång \> principer**
    
2. Välj en princip i listan
    
3. Klicka på **användare och grupper**
    
4. Om du vill ange en viss policy på någon att lägga till dem till **listan** . Om du vill säkerställa att en person utelämnas från principen att lägga till dem i listan **Exkludera** . 
    
Läs mer: [hur du övervaka villkorad tillgång enheter](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

