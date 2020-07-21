---
title: Ta bort överbliven användare från den lokala servern
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198586"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Ta bort överbliven användare från den lokala servern

Så här tar du bort en överbliven användare:

1. Tvinga katalogsynkronisering genom att följa instruktionerna i [Vad är hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Information om hur du verifierar katalogsynkronisering finns i [Vad är hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Om synkroniseringen fungerar korrekt men borttagningen av Active Directory-objekt inte sprids till Azure AD, tar du bort det överblivna objektet manuellt med hjälp av någon av följande Azure Active Directory-modul för Windows PowerShell-cmdlets:

    Ta bort-MsolContact  
    Ta bort-MsolGroup  
    Ta bort MsolUser

    Om du till exempel vill ta bort överblivna användar-ID john.smith@contoso.com, som ursprungligen skapades med hjälp av katalogsynkronisering, kör cmdleten:

    Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com