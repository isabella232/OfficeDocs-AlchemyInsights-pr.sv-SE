---
title: Åtkomst till prenumeration
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807723"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="db03b-102">Det går inte att logga in i Azure på grund av webbläsarens problem (webbläsaren hänger sig, fungerar inte, laddas inte osv.)</span><span class="sxs-lookup"><span data-stu-id="db03b-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="db03b-103">Du kan ha drabbats av ett avbrott.</span><span class="sxs-lookup"><span data-stu-id="db03b-103">You might be impacted by an outage.</span></span> <span data-ttu-id="db03b-104">Kontrol lera om det finns ett pågående avbrott: [Azure Health status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="db03b-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="db03b-105">Logga ut från alla aktiva Azure-sessioner.</span><span class="sxs-lookup"><span data-stu-id="db03b-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="db03b-106">Starta ett privat eller inkognitofönstert läge i webbläsaren.</span><span class="sxs-lookup"><span data-stu-id="db03b-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="db03b-107">Du kan också försöka uppdatera webbläsaren, använda en annan webbläsare och ta bort cache-cookies om ovanstående inte fungerar.</span><span class="sxs-lookup"><span data-stu-id="db03b-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="db03b-108">Läs mer: [Felsöka inloggnings problem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="db03b-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="db03b-109">**Det går inte att komma åt abonnemang**</span><span class="sxs-lookup"><span data-stu-id="db03b-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="db03b-110">I [Azure-portalen](https://portal.azure.com/)kontrollerar du att rätt Azure-katalog är vald från kontot längst upp till höger.</span><span class="sxs-lookup"><span data-stu-id="db03b-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="db03b-111">I [Azure-konto Center](https://account.windowsazure.com/Subscriptions)kontrollerar du att det konto som används är konto administratören.</span><span class="sxs-lookup"><span data-stu-id="db03b-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="db03b-112">Läs mer: [Felsöka inga prenumerationer](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="db03b-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="db03b-113">**Kunde inte komma åt fakturerings historik**</span><span class="sxs-lookup"><span data-stu-id="db03b-113">**Unable to access billing history**</span></span>

<span data-ttu-id="db03b-114">Konto administratören måste kontrol lera att användaren som använder fakturerings informationen läggs till i Azure Active Directory som gäst användare: [lägga till eller ta bort en ny användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="db03b-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="db03b-115">Användaren måste då ges rollen som global administratör: [tilldela användare rollen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="db03b-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="db03b-116">Publicera detta kan användaren få till gång till en debiterings åtkomst med RBAC-principer: [bevilja åtkomst till fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="db03b-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="db03b-117">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="db03b-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="db03b-118">Jag kan inte logga in för att hantera mitt Azure-abonnemang</span><span class="sxs-lookup"><span data-stu-id="db03b-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)