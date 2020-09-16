---
title: Migrering från AIP till MIP/Unified-etiketter i Compliance Center
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674344"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="57cef-102">Migrering från AIP till MIP/Unified-etiketter i Compliance Center</span><span class="sxs-lookup"><span data-stu-id="57cef-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="57cef-103">Om du vill migrera från AIP Labels till Unified Etiketting i säkerhets-och kompatibilitetstillstånd gör du så här:</span><span class="sxs-lookup"><span data-stu-id="57cef-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="57cef-104">**Aktivera skydd från Azure-portalen**</span><span class="sxs-lookup"><span data-stu-id="57cef-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="57cef-105">Om du inte redan har gjort det öppnar du ett nytt webbläsarfönster och loggar in på [Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="57cef-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="57cef-106">Navigera till bladet **Azure information Protection** .</span><span class="sxs-lookup"><span data-stu-id="57cef-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="57cef-107">Klicka till exempel på **alla tjänster** på NAV-menyn och börja skriva in **information** i rutan filter.</span><span class="sxs-lookup"><span data-stu-id="57cef-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="57cef-108">Välj **Azure information Protection**.</span><span class="sxs-lookup"><span data-stu-id="57cef-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="57cef-109">Om du inte har fått åtkomst till bladet Azure information Protection innan kan du se de enskilda [åtgärderna](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) för att lägga till bladet i portalen.</span><span class="sxs-lookup"><span data-stu-id="57cef-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="57cef-110">Om du vill öppna Azure information Protection-bladet måste du ha ett [Azure information Protection Premium-abonnemang](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller ett Office 365-abonnemang som innehåller Rights Management.</span><span class="sxs-lookup"><span data-stu-id="57cef-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="57cef-111">Om du har en av de här prenumerationerna men ser ett meddelande om att det inte går att hitta ett giltigt abonnemang [kontaktar du Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller använder dina Standard Support kanaler.</span><span class="sxs-lookup"><span data-stu-id="57cef-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="57cef-112">Leta reda på Meny alternativen **Hantera** och välj **skydds aktivering**.</span><span class="sxs-lookup"><span data-stu-id="57cef-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="57cef-113">Klicka på **Aktivera**och bekräfta åtgärden.</span><span class="sxs-lookup"><span data-stu-id="57cef-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="57cef-114">När aktiveringen är färdig visar informations fältet **aktiveringen klar**.</span><span class="sxs-lookup"><span data-stu-id="57cef-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="57cef-115">**Migrera Azure information Protection-etiketter till Office 365 Security & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="57cef-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="57cef-116">Kontrol lera att du är inloggad som en användare med global administratörs behörighet.</span><span class="sxs-lookup"><span data-stu-id="57cef-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="57cef-117">Navigera till bladet **Azure information Protection** .</span><span class="sxs-lookup"><span data-stu-id="57cef-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="57cef-118">Välj **Unified etiketting**i menyn **Hantera** .</span><span class="sxs-lookup"><span data-stu-id="57cef-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="57cef-119">På sidan **Azure information Protection-enhetligt etikett** blad klickar du på **Aktivera** och följer instruktionerna online.</span><span class="sxs-lookup"><span data-stu-id="57cef-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="57cef-120">**Obs!** kontrol lera att du har rätt behörighet innan du aktiverar säkerhets &s Center migration.</span><span class="sxs-lookup"><span data-stu-id="57cef-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="57cef-121">Mer information finns i de här artiklarna:</span><span class="sxs-lookup"><span data-stu-id="57cef-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="57cef-122">Måste du vara global administratör för att konfigurera Azure information Protection eller kan jag delegera till andra administratörer?</span><span class="sxs-lookup"><span data-stu-id="57cef-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="57cef-123">Viktig information om administrativa roller efter migrering till säkerhets & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="57cef-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="57cef-124">Mer information om AIP till enhetlig etikett överföring till säkerhets-och efterlevnadsprinciper finns i [migrera etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="57cef-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
