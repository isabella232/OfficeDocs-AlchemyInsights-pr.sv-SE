---
title: Skapa en organisationsrelation så att dina användare kan samarbeta med en annan organisation
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816146"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="6967b-102">Skapa en organisationsrelation så att dina användare kan samarbeta med en annan organisation</span><span class="sxs-lookup"><span data-stu-id="6967b-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="6967b-103">Från instrumentpanelen i administrationscentret för Microsoft 365 går du till **Admin**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="6967b-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="6967b-104">Gå till  >  **organisationsdelning**.</span><span class="sxs-lookup"><span data-stu-id="6967b-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="6967b-105">Klicka **på Nytt** under **Organisationsdelning.**</span><span class="sxs-lookup"><span data-stu-id="6967b-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="6967b-106">Ange **ett eget namn** på **organisationsrelationen i** rutan Relationsnamn i den nya organisationsrelationen.</span><span class="sxs-lookup"><span data-stu-id="6967b-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="6967b-107">I rutan **Domäner att** dela med anger du domänen för den externa office 365- eller Exchange-lokala organisationen som du vill ska kunna se dina kalendrar.</span><span class="sxs-lookup"><span data-stu-id="6967b-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="6967b-108">Om du behöver ange mer än en domän avgränsar du domännamnen med kommatecken.</span><span class="sxs-lookup"><span data-stu-id="6967b-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="6967b-109">Till exempel contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6967b-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="6967b-110">Markera kryssrutan **Aktivera delning av kalenderinformation om du** vill aktivera kalenderdelning med de domäner som du har angett.</span><span class="sxs-lookup"><span data-stu-id="6967b-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="6967b-111">Ange delningsnivå för ledig/upptagen-information och ange vilka användare som kan dela ledig/upptagen-information.</span><span class="sxs-lookup"><span data-stu-id="6967b-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="6967b-112">Välj något av följande för att ställa in åtkomstnivån ledig/upptagen:</span><span class="sxs-lookup"><span data-stu-id="6967b-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="6967b-113">**Ledig/upptagen med information om enbart tid**</span><span class="sxs-lookup"><span data-stu-id="6967b-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="6967b-114">**Kalendern är ledig/upptagen med tid, ämne och plats**</span><span class="sxs-lookup"><span data-stu-id="6967b-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="6967b-115">Välj något av följande om du vill ange vilka användare som ska dela ledig/upptagen-information i kalendern:</span><span class="sxs-lookup"><span data-stu-id="6967b-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="6967b-116">**Alla i organisationen**</span><span class="sxs-lookup"><span data-stu-id="6967b-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="6967b-117">**En angiven säkerhetsgrupp**</span><span class="sxs-lookup"><span data-stu-id="6967b-117">**A specified security group**</span></span>  

<span data-ttu-id="6967b-118">Klicka **på** Bläddra och välj säkerhetsgrupp från en lista och klicka sedan på **OK.**</span><span class="sxs-lookup"><span data-stu-id="6967b-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="6967b-119">Klicka **på Spara** för att skapa en organisationsrelation.</span><span class="sxs-lookup"><span data-stu-id="6967b-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="6967b-120">**Obs!** Konfigurationer mellan klientorganisationen stöder inte personliga kontakter för sökning ledig/upptagen.</span><span class="sxs-lookup"><span data-stu-id="6967b-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="6967b-121">Kontakter måste finnas med i den globala adresslistan för att uppslag som är ledig/upptagen ska fungera.</span><span class="sxs-lookup"><span data-stu-id="6967b-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="6967b-122">**Mer information för fullständig förståelse av det här avsnittet finns här:**</span><span class="sxs-lookup"><span data-stu-id="6967b-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="6967b-123">Skapa en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6967b-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="6967b-124">Ändra en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6967b-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="6967b-125">Ta bort en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6967b-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
