---
title: Migrering från AIP till MIP/Unified Labeling i efterlevnadscentret
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825389"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="0b930-102">Migrering från AIP till MIP/Unified Labeling i efterlevnadscentret</span><span class="sxs-lookup"><span data-stu-id="0b930-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="0b930-103">Så här migrerar du från AIP-etiketter till Unified Labeling i Säkerhets- och efterlevnadscenter:</span><span class="sxs-lookup"><span data-stu-id="0b930-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="0b930-104">**Aktivera skydd från Azure Portal**</span><span class="sxs-lookup"><span data-stu-id="0b930-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="0b930-105">Om du inte redan har gjort det öppnar du ett nytt webbläsarfönster och [loggar in på Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="0b930-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="0b930-106">Gå till **bladet för Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="0b930-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="0b930-107">I till exempel hubb-menyn klickar du **på Alla tjänster** och börjar skriva **Information** i rutan Filter.</span><span class="sxs-lookup"><span data-stu-id="0b930-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="0b930-108">Välj **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="0b930-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="0b930-109">Om du inte har åtkomst till Azure Information Protection-bladet tidigare kan du gå till de ytterligare anvisningarna [för](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) att lägga till det här bladet i portalen.</span><span class="sxs-lookup"><span data-stu-id="0b930-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="0b930-110">För att kunna öppna Azure Information Protection-bladet måste du ha ett [Azure Information Protection Premium-abonnemang](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller ett Office 365-abonnemang som omfattar rättighetshantering.</span><span class="sxs-lookup"><span data-stu-id="0b930-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="0b930-111">Om du har en av dessa prenumerationer men ser ett meddelande om att det inte går att hitta en giltig prenumeration kontaktar du [Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller använder dina standardsupportkanaler.</span><span class="sxs-lookup"><span data-stu-id="0b930-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="0b930-112">Leta reda **på** menyalternativen Hantera och välj **Skyddaktivering**.</span><span class="sxs-lookup"><span data-stu-id="0b930-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="0b930-113">Klicka **på** Aktivera och bekräfta sedan åtgärden.</span><span class="sxs-lookup"><span data-stu-id="0b930-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="0b930-114">När aktiveringen är klar visas aktiveringen **som slutförd i informationsfältet.**</span><span class="sxs-lookup"><span data-stu-id="0b930-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="0b930-115">**Migrera Azure Information Protection-etiketter till Säkerhets- och & Office 365**</span><span class="sxs-lookup"><span data-stu-id="0b930-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="0b930-116">Kontrollera att du är inloggad som användare med behörigheten Global administratör.</span><span class="sxs-lookup"><span data-stu-id="0b930-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="0b930-117">Gå till **bladet för Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="0b930-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="0b930-118">I **menyalternativet** Hantera väljer du **Unified Labeling**.</span><span class="sxs-lookup"><span data-stu-id="0b930-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="0b930-119">I Azure **Information Protection – enhetligt etikettblad klickar** du på Aktivera **och** följer onlineinstruktionerna.</span><span class="sxs-lookup"><span data-stu-id="0b930-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="0b930-120">**Obs!** Kontrollera att du har rätt behörigheter innan du aktiverar migreringen av säkerhets- & säkerhets- och efterlevnadscentret.</span><span class="sxs-lookup"><span data-stu-id="0b930-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="0b930-121">Mer information finns i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="0b930-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="0b930-122">Behöver du vara global administratör för att konfigurera Azure Information Protection, eller kan jag delegera till andra administratörer?</span><span class="sxs-lookup"><span data-stu-id="0b930-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="0b930-123">Viktig information om administrativa roller efter migrering till Säkerhets- & Efterlevnadscenter.</span><span class="sxs-lookup"><span data-stu-id="0b930-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="0b930-124">Mer information om migrering av AIP till Unified Labeling till Säkerhets- och efterlevnadscenter finns i [Migrera etiketter.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="0b930-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
