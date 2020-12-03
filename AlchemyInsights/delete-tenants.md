---
title: Ta bort klient organisation
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564879"
---
# <a name="delete-tenant"></a><span data-ttu-id="e9190-102">Ta bort klient organisation</span><span class="sxs-lookup"><span data-stu-id="e9190-102">Delete tenant</span></span>

<span data-ttu-id="e9190-103">Kontrol lera följande om du vill ta bort en Azure-annons:</span><span class="sxs-lookup"><span data-stu-id="e9190-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="e9190-104">Du är global administratör för katalogen.</span><span class="sxs-lookup"><span data-stu-id="e9190-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="e9190-105">Du är inte inloggad med ett konto som har standard katalogen, till exempel contoso.onmicrosoft.com i det signerade kontot, till exempel admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="e9190-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="e9190-106">Ta bort alla aktiva program i katalogen innan du raderas.</span><span class="sxs-lookup"><span data-stu-id="e9190-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="e9190-107">Om du vill ta bort aktiva program navigerar du till program registreringar och tar bort befintliga program.</span><span class="sxs-lookup"><span data-stu-id="e9190-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="e9190-108">Det finns inga aktiva abonnemang för alla Microsoft Online-tjänster, till exempel Microsoft Azure, Office 365 eller Azure AD Premium som är kopplade till katalogen.</span><span class="sxs-lookup"><span data-stu-id="e9190-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="e9190-109">Överför dina abonnemang eller påskynda annulleringen av aktiva abonnemang via Azure-support och fakturering.</span><span class="sxs-lookup"><span data-stu-id="e9190-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="e9190-110">Läs mer om hur du avbryter Office 365-och Azure-prenumerationer.</span><span class="sxs-lookup"><span data-stu-id="e9190-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="e9190-111">Råd om att associera eller lägga till en befintlig prenumeration på en klient organisation finns i [associera eller lägga till ett Azure-abonnemang till din Azure AD-klient](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="e9190-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="e9190-112">Det finns ingen aktiv licens.</span><span class="sxs-lookup"><span data-stu-id="e9190-112">There are no Active license.</span></span> <span data-ttu-id="e9190-113">Om du vill ta bort licenser läser du [ta bort abonnemang för att ta bort licensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="e9190-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="e9190-114">Det finns inga andra aktiva användare i katalogen förutom dig själv som global administratör när du försöker ta bort Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e9190-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="e9190-115">Ta bort alla andra aktiva användare och eventuella beroenden för ett anpassat domän namn i klient organisationen måste också tas bort, till exempel användare som skapats med admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="e9190-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="e9190-116">Mer information om hur du:</span><span class="sxs-lookup"><span data-stu-id="e9190-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="e9190-117">Ta bort "Azure Active Directory" eller "prenumeration", se [ta bort Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="e9190-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="e9190-118">Ta bort program i katalogen finns i [ta bort program](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="e9190-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
