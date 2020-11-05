---
title: Moderna Azure e-postfakturering
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922145"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="8f41e-102">E-postfakturering i Azure</span><span class="sxs-lookup"><span data-stu-id="8f41e-102">Email invoicing in Azure</span></span>

<span data-ttu-id="8f41e-103">Du måste ha en ägare eller deltagar roll i fakturerings profilen eller dess fakturerings konto för att kunna uppdatera e-postfakturans preferens.</span><span class="sxs-lookup"><span data-stu-id="8f41e-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="8f41e-104">När du har valt det får alla användare med rollerna ägare, deltagare, läsare och faktura chef i en fakturerings profil sin faktura via e-post.</span><span class="sxs-lookup"><span data-stu-id="8f41e-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="8f41e-105">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8f41e-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8f41e-106">Sök efter **kostnads hantering + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8f41e-107">Välj **fakturor** till vänster och välj sedan **e-postfaktura** längst upp på sidan.</span><span class="sxs-lookup"><span data-stu-id="8f41e-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="8f41e-108">Om du har flera fakturerings profiler väljer du en fakturerings profil och väljer sedan **opt in**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="8f41e-109">Välj **Uppdatera**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-109">Select **Update**.</span></span>
6. <span data-ttu-id="8f41e-110">Om du har flera fakturerings profiler väljer du en fakturerings profil och väljer sedan **opt in**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="8f41e-111">Du ger andra till gång till Visa, ladda ned och betala fakturor genom att tilldela dem rollen som faktura chef för en betalnings profil för MCA eller MPA.</span><span class="sxs-lookup"><span data-stu-id="8f41e-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="8f41e-112">Om du har valt att få fakturan i ett e-postmeddelande får användarna också fakturor via e-post.</span><span class="sxs-lookup"><span data-stu-id="8f41e-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="8f41e-113">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8f41e-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8f41e-114">Sök efter **kostnads hantering + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8f41e-115">Välj **betalnings profiler** från vänster sida.</span><span class="sxs-lookup"><span data-stu-id="8f41e-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="8f41e-116">I listan betalnings profiler väljer du en betalnings profil som du vill tilldela en faktura administratörs roll.</span><span class="sxs-lookup"><span data-stu-id="8f41e-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="8f41e-117">Välj **åtkomst kontroll (IAM)** från den vänstra sidan och välj sedan **Lägg till** högst upp på sidan.</span><span class="sxs-lookup"><span data-stu-id="8f41e-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="8f41e-118">I list rutan Role väljer du **faktura chef**.</span><span class="sxs-lookup"><span data-stu-id="8f41e-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="8f41e-119">Ange e-postadressen för den användare som ska ge åtkomst.</span><span class="sxs-lookup"><span data-stu-id="8f41e-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="8f41e-120">Välj **Spara** för att tilldela rollen.</span><span class="sxs-lookup"><span data-stu-id="8f41e-120">Select **Save** to assign the role.</span></span>
