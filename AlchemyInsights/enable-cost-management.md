---
title: Aktivera kostnads hantering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678773"
---
# <a name="enable-cost-management"></a><span data-ttu-id="d09c9-102">Aktivera kostnads hantering</span><span class="sxs-lookup"><span data-stu-id="d09c9-102">Enable cost management</span></span>

<span data-ttu-id="d09c9-103">**Vad innebär "kostnaderna är inaktiverade för din organisation"?**</span><span class="sxs-lookup"><span data-stu-id="d09c9-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="d09c9-104">Organisationer som använder Enterprise Agreement (EA) eller Microsoft Customer Agreement (MCA)-konton kan förhindra åtkomst till information om kostnader och priser.</span><span class="sxs-lookup"><span data-stu-id="d09c9-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="d09c9-105">När du har loggat in på Azure Portal kan de använda API-gränssnitten för att programmatiskt skaffa fakturor (när du har valt) och användnings uppgifter.</span><span class="sxs-lookup"><span data-stu-id="d09c9-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="d09c9-106">**Så här tillåter du fler användare att få åtkomst till fakturor**</span><span class="sxs-lookup"><span data-stu-id="d09c9-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="d09c9-107">Gå till **prenumerationens blad** i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d09c9-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="d09c9-108">Välj **fakturor** och sedan **åtkomst till fakturor**.</span><span class="sxs-lookup"><span data-stu-id="d09c9-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="d09c9-109">Aktivera åtkomst och följ sedan de ändringar du vill göra för att tillåta användare i prenumerations bara roller att ladda ner fakturor.</span><span class="sxs-lookup"><span data-stu-id="d09c9-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="d09c9-110">Konto administratören kan också konfigurera så att fakturor skickas via e-post.</span><span class="sxs-lookup"><span data-stu-id="d09c9-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="d09c9-111">Mer information finns i [Hämta din faktura via e-post](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="d09c9-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="d09c9-112">**Så här lägger du till användare i rollen fakturerings läsare**</span><span class="sxs-lookup"><span data-stu-id="d09c9-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="d09c9-113">Gå till **prenumerationens blad** i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d09c9-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="d09c9-114">Välj **åtkomst kontroll (IAM)** och klicka sedan på **Lägg till**.</span><span class="sxs-lookup"><span data-stu-id="d09c9-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="d09c9-115">Välj **fakturerings läsare** på sidan **Välj en roll** .</span><span class="sxs-lookup"><span data-stu-id="d09c9-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="d09c9-116">Skriv e-postmeddelandet för den användare som du vill bjuda in och klicka sedan på **OK** för att skicka inbjudan.</span><span class="sxs-lookup"><span data-stu-id="d09c9-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="d09c9-117">Följ instruktionerna i inbjudan via e-post om du vill logga in som en fakturerings läsare.</span><span class="sxs-lookup"><span data-stu-id="d09c9-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="d09c9-118">Mer information finns i [bevilja åtkomst till fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="d09c9-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="d09c9-119">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="d09c9-119">**Recommended documents**</span></span>

- [<span data-ttu-id="d09c9-120">Aktivera DA-och AO-vyer via EA-portalen</span><span class="sxs-lookup"><span data-stu-id="d09c9-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="d09c9-121">Kostnader inkluderade i kostnads hantering</span><span class="sxs-lookup"><span data-stu-id="d09c9-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="d09c9-122">Support för Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d09c9-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="d09c9-123">Granska kostnader i kostnads analys</span><span class="sxs-lookup"><span data-stu-id="d09c9-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="d09c9-124">Ge åtkomst till fakturerings uppgifter</span><span class="sxs-lookup"><span data-stu-id="d09c9-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="d09c9-125">Kontrol lera åtkomsten till ett Microsoft-kundavtal</span><span class="sxs-lookup"><span data-stu-id="d09c9-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






