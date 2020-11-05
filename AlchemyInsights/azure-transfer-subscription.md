---
title: Överför ägandes Kap för Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922171"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="9132d-102">Överför ägandes Kap för Azure</span><span class="sxs-lookup"><span data-stu-id="9132d-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="9132d-103">Logga in på [Azure-portalen](https://portal.azure.com/) som administratör för det fakturerings konto som har den prenumeration du vill överföra.</span><span class="sxs-lookup"><span data-stu-id="9132d-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="9132d-104">Om du är osäker på om du är och administratör, eller om du behöver ta reda på vem som är, kan du läsa [kontrol lera konto fakturerings administratör](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="9132d-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="9132d-105">Sök på **kostnads hantering + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="9132d-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="9132d-106">Välj **prenumerationer** från vänster fönster ruta.</span><span class="sxs-lookup"><span data-stu-id="9132d-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="9132d-107">Beroende på åtkomst kan du behöva välja en fakturerings omfattning och sedan **prenumerationer** eller **Azure-prenumerationer**.</span><span class="sxs-lookup"><span data-stu-id="9132d-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="9132d-108">Välj **överför ägandes Kap** för abonnemanget som du vill överföra</span><span class="sxs-lookup"><span data-stu-id="9132d-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="9132d-109">Ange e-postadressen för en användare som är fakturerings administratör för det konto som kommer att bli den nya ägaren för abonnemanget och sedan välja **Skicka överförings förfrågan**</span><span class="sxs-lookup"><span data-stu-id="9132d-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="9132d-110">Användaren får ett e-postmeddelande med instruktioner för att kontrol lera din överföringsbegäran.</span><span class="sxs-lookup"><span data-stu-id="9132d-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="9132d-111">För att godkänna överföringsbegäran väljer användaren länken i e-postmeddelandet och följer anvisningarna.</span><span class="sxs-lookup"><span data-stu-id="9132d-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="9132d-112">**Obs!** om du överför fakturerings ägandet för ditt abonnemang till en användares konto i en annan Azure AD-klient organisation, tas alla aktiviteter för [rollbaserad åtkomst kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)för att hantera resurser i prenumerationen permanent bort.</span><span class="sxs-lookup"><span data-stu-id="9132d-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="9132d-113">Endast den nya ägaren får åtkomst till att hantera resurser i prenumerationen.</span><span class="sxs-lookup"><span data-stu-id="9132d-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="9132d-114">Mer information finns i [överföra ett abonnemang till en användare i en annan Azure AD-klient organisation](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9132d-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9132d-115">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="9132d-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="9132d-116">Överföra fakturerings ägandes Kap för ett Azure-abonnemang till ett annat konto</span><span class="sxs-lookup"><span data-stu-id="9132d-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="9132d-117">Om att överföra ägandes Kap till en Azure-prenumeration</span><span class="sxs-lookup"><span data-stu-id="9132d-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="9132d-118">Överför Visual Studio, Microsoft Partner Network (MPN) och betala allt eftersom med prov abonnemang</span><span class="sxs-lookup"><span data-stu-id="9132d-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="9132d-119">Vanliga frågor och svar om ägarskap</span><span class="sxs-lookup"><span data-stu-id="9132d-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="9132d-120">Felsöka problem med överförings ägarskap</span><span class="sxs-lookup"><span data-stu-id="9132d-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
