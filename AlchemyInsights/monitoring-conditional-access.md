---
title: Övervakning av villkorad tillgång
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538793"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervakning av villkorlig åtkomst för Exchange

Riktade med villkorad tillgång användare får ett e-postmeddelanden om de inte uppfyller kraven i din organisation åtkomst. Lös, rekommenderar vi en eller flera av följande lösningar:
  
- Om enheten antas vara anmäld, informera användaren att gå till appen företagsportal och kontrollera att det visas i företagets Portal. Användaren bör registrera enheten om den inte.
    
- Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **enheten överensstämmelse**under **Bildskärm** . Visa enheten överensstämmelse rapporten för att kontrollera att användarens enhet är markerad som kompatibla. 
    
- Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **principer**under **Hantera**. I listan över principer för att kontrollera att en profil har tilldelats användarens enhet. Om ingen profil tilldelas Intune inte bekräfta överensstämmelse Enhetsstatus. 
    
- Redigera Användartilldelning villkorad tillgång.
    
1. Gå till Azure portal **Intune \> villkorad tillgång \> principer**
    
2. Välj en princip i listan
    
3. Klicka på **användare och grupper**
    
4. Om du vill ange en viss policy på någon att lägga till dem till **listan** . Om du vill säkerställa att en person utelämnas från principen att lägga till dem i listan **Exkludera** . 
    
Läs mer: [hur du övervaka villkorad tillgång enheter](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

