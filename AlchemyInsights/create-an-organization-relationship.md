---
title: Skapa en organisationsrelation så att användarna kan samarbeta med en annan organisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862192"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="b02a8-102">Skapa en organisationsrelation så att användarna kan samarbeta med en annan organisation</span><span class="sxs-lookup"><span data-stu-id="b02a8-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="b02a8-103">Gå till **Admin**Exchange på instrumentpanelen i Microsoft 365 admin center  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b02a8-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="b02a8-104">Gå **organization**till  >  **organisationsdelning**.</span><span class="sxs-lookup"><span data-stu-id="b02a8-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="b02a8-105">Klicka på **Nytt** under **Organisationsdelning.**</span><span class="sxs-lookup"><span data-stu-id="b02a8-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="b02a8-106">I **den nya organisationsrelationen**skriver du ett eget namn för organisationsrelationen i rutan **Relationnamn.**</span><span class="sxs-lookup"><span data-stu-id="b02a8-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="b02a8-107">I rutan **Domäner som ska delas med** skriver du domänen för den externa office 365- eller Exchange-organisation som du vill att dina kalendrar ska visas.</span><span class="sxs-lookup"><span data-stu-id="b02a8-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="b02a8-108">Om du behöver ange mer än en domän avgränsar du domännamnen med ett kommatecken.</span><span class="sxs-lookup"><span data-stu-id="b02a8-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="b02a8-109">Till exempel contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b02a8-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="b02a8-110">Markera kryssrutan **Aktivera ledig/upptagen-informationsdelning** i kalendern om du vill aktivera kalenderdelning med de domäner som du listade.</span><span class="sxs-lookup"><span data-stu-id="b02a8-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="b02a8-111">Ange delningsnivån för ledig/upptagen-information i kalendern och ange vilka användare som kan dela ledig/upptagen-information i kalendern.</span><span class="sxs-lookup"><span data-stu-id="b02a8-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="b02a8-112">Om du vill ange ledig/upptagen åtkomstnivå väljer du något av följande:</span><span class="sxs-lookup"><span data-stu-id="b02a8-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="b02a8-113">**Ledig/upptagen med information om enbart tid**</span><span class="sxs-lookup"><span data-stu-id="b02a8-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="b02a8-114">**Kalender ledig/upptagen med tid, ämne och plats**</span><span class="sxs-lookup"><span data-stu-id="b02a8-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="b02a8-115">Om du vill ange vilka användare som ska dela ledig/upptagen-information i kalendern väljer du något av följande:</span><span class="sxs-lookup"><span data-stu-id="b02a8-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="b02a8-116">**Alla i organisationen**</span><span class="sxs-lookup"><span data-stu-id="b02a8-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="b02a8-117">**En angiven säkerhetsgrupp**</span><span class="sxs-lookup"><span data-stu-id="b02a8-117">**A specified security group**</span></span>  

<span data-ttu-id="b02a8-118">Klicka **på Bläddra** för att välja säkerhetsgruppen från en lista och klicka sedan på **ok**.</span><span class="sxs-lookup"><span data-stu-id="b02a8-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="b02a8-119">Klicka på **Spara** för att skapa organisationsrelationen.</span><span class="sxs-lookup"><span data-stu-id="b02a8-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="b02a8-120">**Obs:** Konfigurationer mellan klienter stöder inte personliga kontakter för ledig/upptagen sökning.</span><span class="sxs-lookup"><span data-stu-id="b02a8-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="b02a8-121">Kontakter måste inkluderas i den globala adresslistan för att ledig/upptagen-sökning ska fungera.</span><span class="sxs-lookup"><span data-stu-id="b02a8-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="b02a8-122">**För full förståelse för detta ämne läs:**</span><span class="sxs-lookup"><span data-stu-id="b02a8-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="b02a8-123">Skapa en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b02a8-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="b02a8-124">Ändra en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b02a8-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="b02a8-125">Ta bort en organisationsrelation i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b02a8-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
