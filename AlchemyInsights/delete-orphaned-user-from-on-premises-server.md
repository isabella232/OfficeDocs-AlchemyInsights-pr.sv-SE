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
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="8064f-102">Ta bort överbliven användare från den lokala servern</span><span class="sxs-lookup"><span data-stu-id="8064f-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="8064f-103">Så här tar du bort en överbliven användare:</span><span class="sxs-lookup"><span data-stu-id="8064f-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="8064f-104">Tvinga katalogsynkronisering genom att följa instruktionerna i [Vad är hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="8064f-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="8064f-105">Information om hur du verifierar katalogsynkronisering finns i [Vad är hybrididentitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="8064f-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="8064f-106">Om synkroniseringen fungerar korrekt men borttagningen av Active Directory-objekt inte sprids till Azure AD, tar du bort det överblivna objektet manuellt med hjälp av någon av följande Azure Active Directory-modul för Windows PowerShell-cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8064f-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="8064f-107">Ta bort-MsolContact</span><span class="sxs-lookup"><span data-stu-id="8064f-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="8064f-108">Ta bort-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="8064f-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="8064f-109">Ta bort MsolUser</span><span class="sxs-lookup"><span data-stu-id="8064f-109">Remove-MsolUser</span></span>

    <span data-ttu-id="8064f-110">Om du till exempel vill ta bort överblivna användar-ID john.smith@contoso.com, som ursprungligen skapades med hjälp av katalogsynkronisering, kör cmdleten:</span><span class="sxs-lookup"><span data-stu-id="8064f-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="8064f-111">Remove-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="8064f-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>