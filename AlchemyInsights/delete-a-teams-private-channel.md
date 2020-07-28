---
title: Ta bort en privat teams-kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439913"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="c080f-102">Ta bort en privat teams-kanal</span><span class="sxs-lookup"><span data-stu-id="c080f-102">Delete a Teams private channel</span></span>

<span data-ttu-id="c080f-103">Microsoft är medvetet om ett problem med att ta bort en privat Teams-kanal om du har aktiverat SharePoint-bevarandeprinciper för den underliggande SharePoint-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="c080f-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="c080f-104">Microsoft arbetar på en fix.</span><span class="sxs-lookup"><span data-stu-id="c080f-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="c080f-105">Under tiden kan du använda följande lösningar för att ta bort den privata kanalen.</span><span class="sxs-lookup"><span data-stu-id="c080f-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="c080f-106">**Uteslut grupp-/webbplatssamlingen från principen för lagring av Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="c080f-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="c080f-107">Gå till administrationsportalen för Office 365 och välj **Visa alla** i det vänstra navigeringsfönstret.</span><span class="sxs-lookup"><span data-stu-id="c080f-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="c080f-108">Under **Administrationscenter**går du till **Säkerhet & policy för**att förhindra  >  **efterlevnadsdataförlust**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="c080f-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="c080f-109">Identifiera alla policyer som gäller för Sharepoint-webbplatser och ändra principen så att Sharepoint-webbplatsen för teamet som innehåller den privata kanalen INTE inkluderas i bevarandeprincipen.</span><span class="sxs-lookup"><span data-stu-id="c080f-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="c080f-110">Spara principen.</span><span class="sxs-lookup"><span data-stu-id="c080f-110">Save the policy.</span></span>
    <span data-ttu-id="c080f-111">Det kan ta upp till 24 timmar innan principinställningarna börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="c080f-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="c080f-112">När webbplatsen har uteslutits kan du ta bort den privata kanalen.</span><span class="sxs-lookup"><span data-stu-id="c080f-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="c080f-113">Du ***kanske kan*** ta bort den privata kanalen med hjälp av Microsoft Teams på din Android-enhet.</span><span class="sxs-lookup"><span data-stu-id="c080f-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="c080f-114">Relaterad SharePoint-information finns [i Det går inte att ta bort objekt i SharePoint Online eller OneDrive för företag](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="c080f-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>