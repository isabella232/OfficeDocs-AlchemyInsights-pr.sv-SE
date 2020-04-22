---
title: Övervaka villkorlig åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713736"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervaka villkorlig åtkomst för Exchange

Användare som är inriktade på villkorlig åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav. För att lösa det rekommenderar vi en eller flera av följande lösningar:
  
- Om enheten antas vara registrerad, råda användaren att gå till företagsportalappen och kontrollera att den visas i företagsportalen. Om den inte gör det bör användaren registrera enheten.
    
- Gå till **Intune \> Device compliance**i Azure-portalen . Klicka på **Enhetsefterlevnad**under **Bildskärm.** Visa enhetens efterlevnadsrapport för att kontrollera att användarens enhet är markerad som kompatibel. 
    
- Gå till **Intune \> Device compliance**i Azure-portalen . Klicka på **Principer**under **Hantera.** Kontrollera att en profil har tilldelats användarens enhet i listan över efterlevnadsprinciper. Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus. 
    
- Redigera användarens tilldelning av villkorlig åtkomst.
    
1. Gå till **Intune-principer \> för \> villkorlig åtkomst i** Azure-portalen
    
2. Välj en princip i listan
    
3. Klicka på **Användare och grupper**
    
4. Om du vill rikta en viss princip mot någon lägger du till dem i listan **Inkludera.** Om du vill vara säkra på att en person utelämnas från principen lägger du till dem i listan **Uteslut.** 
    
Läs mer: [Så här övervakar du enheter med villkorlig åtkomst](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

