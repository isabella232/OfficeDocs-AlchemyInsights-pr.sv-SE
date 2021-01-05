---
title: Så här lägger du till och hanterar administratörer
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755529"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="01b68-102">Så här lägger du till och hanterar administratörer</span><span class="sxs-lookup"><span data-stu-id="01b68-102">How to add and manage admins</span></span>

<span data-ttu-id="01b68-103">Vi har hittat en lösning på problemet.</span><span class="sxs-lookup"><span data-stu-id="01b68-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="01b68-104">De flesta kunder kunde lösa sina problem efter att ha följt vår dokumentation.</span><span class="sxs-lookup"><span data-stu-id="01b68-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="01b68-105">För att hantera ditt fakturerings konto för ett Microsoft Customer Agreement (MCA) kan du använda olika roller med den önskade åtkomst nivån.</span><span class="sxs-lookup"><span data-stu-id="01b68-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="01b68-106">Dessa roller är utöver de inbyggda Azure Service roles som hjälper dig att kontrol lera dina resurser.</span><span class="sxs-lookup"><span data-stu-id="01b68-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="01b68-107">**Så här lägger du till fakturerings roller i Azure-portalen:**</span><span class="sxs-lookup"><span data-stu-id="01b68-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="01b68-108">Logga in på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="01b68-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="01b68-109">Sök efter *kostnads hantering + fakturering*.</span><span class="sxs-lookup"><span data-stu-id="01b68-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="01b68-110">Välj åtkomst kontroll (IAM) i ett scope som fakturerings konto, fakturerings profil eller faktura avsnitt där du vill ge åtkomst.</span><span class="sxs-lookup"><span data-stu-id="01b68-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="01b68-111">På sidan åtkomst kontroll (IAM) visas användare och grupper som är tilldelade till varje roll för det aktuella området.</span><span class="sxs-lookup"><span data-stu-id="01b68-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="01b68-112">Om du vill ge åtkomst till en användare väljer du **Lägg till** högst upp på sidan.</span><span class="sxs-lookup"><span data-stu-id="01b68-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="01b68-113">I list rutan *Role* väljer du en roll.</span><span class="sxs-lookup"><span data-stu-id="01b68-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="01b68-114">Ange e-postadressen till den användare som du vill ge åtkomst till.</span><span class="sxs-lookup"><span data-stu-id="01b68-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="01b68-115">Välj **Spara** för att tilldela rollen.</span><span class="sxs-lookup"><span data-stu-id="01b68-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="01b68-116">Om du vill ta bort en användares åtkomst markerar du användaren med den roll tilldelning du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="01b68-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="01b68-117">Välj **ta bort**.</span><span class="sxs-lookup"><span data-stu-id="01b68-117">Select **Remove**.</span></span>

<span data-ttu-id="01b68-118">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="01b68-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="01b68-119">Roll definitioner för fakturering</span><span class="sxs-lookup"><span data-stu-id="01b68-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="01b68-120">Roller och uppgifter för fakturerings konto</span><span class="sxs-lookup"><span data-stu-id="01b68-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="01b68-121">Komma igång med ditt MCA-konto</span><span class="sxs-lookup"><span data-stu-id="01b68-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="01b68-122">Kontrol lera åtkomsten till ett Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="01b68-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
