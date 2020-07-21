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
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="9cf57-102">Användaren får fel AADSTS7000112 Yammer är inaktiverad</span><span class="sxs-lookup"><span data-stu-id="9cf57-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="9cf57-103">Om felet "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-000000000000000000000000000 är inaktiverat", finns ett problem med tjänstens huvudnamn i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9cf57-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="9cf57-104">En administratör kan ha inaktiverat tjänstens huvudnamn för att blockera åtkomst till Yammer.</span><span class="sxs-lookup"><span data-stu-id="9cf57-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="9cf57-105">Det rekommenderas inte att tjänstens huvudnamn inaktiveras och kan orsaka ytterligare problem.</span><span class="sxs-lookup"><span data-stu-id="9cf57-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="9cf57-106">Mer information om metoden som stöds för att blockera användaråtkomst till Yammer finns i [Inaktivera Yammer-åtkomst för Microsoft 365-användare](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="9cf57-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="9cf57-107">Så här korrigerar du problemet i Azure Portal och återställer användaråtkomst till Yammer:</span><span class="sxs-lookup"><span data-stu-id="9cf57-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="9cf57-108">Öppna sidan Azure Active Directory och välj **Enterprise-program** under **Hantera** i det vänstra navigeringsfönstret.</span><span class="sxs-lookup"><span data-stu-id="9cf57-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="9cf57-109">Skriv **Office 365 Yammer** i sökrutan och välj programnamnet för att öppna inställningarna.</span><span class="sxs-lookup"><span data-stu-id="9cf57-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="9cf57-110">Välj **Egenskaper** under **Hantera** i det vänstra navigeringsfönstret.</span><span class="sxs-lookup"><span data-stu-id="9cf57-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="9cf57-111">Ange värdet **för Aktiverat för användare att logga in?** **Yes** **Save**</span><span class="sxs-lookup"><span data-stu-id="9cf57-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="9cf57-112">Logga in på Yammer igen.</span><span class="sxs-lookup"><span data-stu-id="9cf57-112">Sign in to Yammer again.</span></span> <span data-ttu-id="9cf57-113">Du kan behöva rensa cookies.</span><span class="sxs-lookup"><span data-stu-id="9cf57-113">You might need to clear cookies.</span></span>

<span data-ttu-id="9cf57-114">Du kan också köra PowerShell-kommandon för att ange värdet.</span><span class="sxs-lookup"><span data-stu-id="9cf57-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="9cf57-115">Mer information finns i [Felet "Tyvärr, men vi har problem med att logga in dig" när du klickar på Yammer-panelen i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9cf57-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 