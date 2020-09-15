---
title: Övervaka villkorlig åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702921"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Övervaka villkorlig åtkomst för Exchange

Användare riktade mot villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller åtkomst kraven för organisationen. För att lösa problemet rekommenderar vi en eller flera av följande lösningar:
  
- Om enheten är registrerad kan du uppmana användaren att gå till företagsportalsappen och kontrol lera att den visas i företags portalen. Om det inte gör det bör användaren registrera enheten.
    
- I Azure-portalen går du till **Intune- \> enhetsupptäckning**. Klicka på **enhets överensstämmelse**under **bildskärm** . Visa din enhets kompatibilitetsstatus för att kontrol lera att användarens enhet är markerad som kompatibel. 
    
- I Azure-portalen går du till **Intune- \> enhetsupptäckning**. Under **Hantera**klickar du på **principer**. I listan över efterlevnadsprinciper kontrollerar du att en profil har tilldelats till din användares enhet. Om ingen profil är tilldelad kan Intune inte bekräfta status för enhetens efterlevnad. 
    
- Redigera användarens villkorliga åtkomst tilldelning.
    
1. I Azure-portalen går du till **Intune \> \> policy för villkorsstyrd åtkomst**
    
2. Välj en princip i listan
    
3. Klicka på **användare och grupper**
    
4. Om du vill rikta en viss princip till någon kan du lägga till dem i listan **ta med** . Om du vill se till att en person utelämnas från policyn lägger du till den i listan **undantag** . 
    
Läs mer: [så här övervakar du enheter för villkorsstyrd åtkomst](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

