---
title: Användaren får fel AADSTS7000112 Yammer är inaktiverad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198370"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Användaren får fel AADSTS7000112 Yammer är inaktiverad

Om felet "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-000000000000000000000000000 är inaktiverat", finns ett problem med tjänstens huvudnamn i Azure AD. En administratör kan ha inaktiverat tjänstens huvudnamn för att blockera åtkomst till Yammer.

Det rekommenderas inte att tjänstens huvudnamn inaktiveras och kan orsaka ytterligare problem. Mer information om metoden som stöds för att blockera användaråtkomst till Yammer finns i [Inaktivera Yammer-åtkomst för Microsoft 365-användare](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Så här korrigerar du problemet i Azure Portal och återställer användaråtkomst till Yammer:

1.  Öppna sidan Azure Active Directory och välj **Enterprise-program** under **Hantera** i det vänstra navigeringsfönstret.
3.  Skriv **Office 365 Yammer** i sökrutan och välj programnamnet för att öppna inställningarna.
4.  Välj **Egenskaper** under **Hantera** i det vänstra navigeringsfönstret.
5.  Ange värdet **för Aktiverat för användare att logga in?** **Yes** **Save**
6.  Logga in på Yammer igen. Du kan behöva rensa cookies.

Du kan också köra PowerShell-kommandon för att ange värdet. Mer information finns i [Felet "Tyvärr, men vi har problem med att logga in dig" när du klickar på Yammer-panelen i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 