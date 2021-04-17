---
title: Modern e-postfakturering i Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820844"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="0ee13-102">E-postfakturering i Azure</span><span class="sxs-lookup"><span data-stu-id="0ee13-102">Email invoicing in Azure</span></span>

<span data-ttu-id="0ee13-103">Du måste ha en ägar- eller en deltagarroll i faktureringsprofilen eller det tillhörande faktureringskontot för att kunna uppdatera inställningen för e-postfakturering.</span><span class="sxs-lookup"><span data-stu-id="0ee13-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="0ee13-104">När du har anmält dig får alla användare med en ägar-, deltagar-, läsar- och fakturahanteringsroller i en faktureringsprofil fakturan via e-post.</span><span class="sxs-lookup"><span data-stu-id="0ee13-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="0ee13-105">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0ee13-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0ee13-106">Sök på **Kostnadshantering + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0ee13-107">Välj **Fakturor** på den vänstra sidan och välj sedan **E-postfaktura** högst upp på sidan.</span><span class="sxs-lookup"><span data-stu-id="0ee13-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="0ee13-108">Om du har flera faktureringsprofiler väljer du en faktureringsprofil och väljer sedan **Anmäl dig**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="0ee13-109">Välj **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-109">Select **Update**.</span></span>
6. <span data-ttu-id="0ee13-110">Om du har flera faktureringsprofiler markerar du en faktureringsprofil och väljer sedan **Anmäl dig**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="0ee13-111">Du ger andra tillgång till att visa, ladda ned och betala fakturor genom att tilldela dem rollen som fakturahanterare för en MCA- eller MPA-faktureringsprofil.</span><span class="sxs-lookup"><span data-stu-id="0ee13-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="0ee13-112">Om du har valt att hämta fakturan via e-post får även användarna sina fakturor via e-post.</span><span class="sxs-lookup"><span data-stu-id="0ee13-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="0ee13-113">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0ee13-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0ee13-114">Sök på **Kostnadshantering + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0ee13-115">Markera **Faktureringsprofiler** på den vänstra sidan.</span><span class="sxs-lookup"><span data-stu-id="0ee13-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="0ee13-116">Markera en faktureringsprofil i listan med faktureringsprofiler som du vill tilldela en fakturahanteringsroll.</span><span class="sxs-lookup"><span data-stu-id="0ee13-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="0ee13-117">Markera **Åtkomstkontroll (IAM)** på den vänstra sidan och markera sedan **Lägg till** högst upp på sidan.</span><span class="sxs-lookup"><span data-stu-id="0ee13-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="0ee13-118">I listrutan Roll markerar du **Fakturahanterare**.</span><span class="sxs-lookup"><span data-stu-id="0ee13-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="0ee13-119">Ange användarens e-postadress för att ge åtkomst.</span><span class="sxs-lookup"><span data-stu-id="0ee13-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="0ee13-120">Markera **Spara** för att tilldela rollen.</span><span class="sxs-lookup"><span data-stu-id="0ee13-120">Select **Save** to assign the role.</span></span>
