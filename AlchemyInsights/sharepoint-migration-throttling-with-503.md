---
title: Resursmigreringsbegränsning med 503 fel
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931676"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="e6893-102">Resursmigreringsbegränsning med 503 fel</span><span class="sxs-lookup"><span data-stu-id="e6893-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="e6893-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="e6893-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e6893-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="e6893-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e6893-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="e6893-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e6893-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="e6893-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e6893-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="e6893-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e6893-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="e6893-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e6893-109">**503 fel vid migrering till SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="e6893-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="e6893-110">Det verkar som om du migrerar till SharePoint Online och tar emot 503 fel.</span><span class="sxs-lookup"><span data-stu-id="e6893-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="e6893-111">Följ stegen nedan så att vi kan hjälpa dig så snart som möjligt.</span><span class="sxs-lookup"><span data-stu-id="e6893-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="e6893-112">Klicka på **Kontakta support**och sedan på **Ny servicebegäran**.</span><span class="sxs-lookup"><span data-stu-id="e6893-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="e6893-113">Om du vill ange rubrik och beskrivning skriver du **SharePoint-migreringsbegränsning med 503**.</span><span class="sxs-lookup"><span data-stu-id="e6893-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="e6893-114">När biljetten har skickats, vänligen uppdatera den med följande information:</span><span class="sxs-lookup"><span data-stu-id="e6893-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="e6893-115">Hur mycket kvar av migrering (till exempel hur många TBs?).</span><span class="sxs-lookup"><span data-stu-id="e6893-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="e6893-116">Start- och slutdatum för migrering.</span><span class="sxs-lookup"><span data-stu-id="e6893-116">Migration start and end date.</span></span>
    - <span data-ttu-id="e6893-117">Beskriv var du migrerar ditt innehåll från, till exempel SharePoint Server, Box, GDrive, Filresurser osv..</span><span class="sxs-lookup"><span data-stu-id="e6893-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="e6893-118">Uppskatta antalet begränsningsfel (till exempel x begränsning per timme?) och när skedde begränsningen.</span><span class="sxs-lookup"><span data-stu-id="e6893-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="e6893-119">Vilket migreringsverktyg du använder (till exempel SPMT eller ShareGate).</span><span class="sxs-lookup"><span data-stu-id="e6893-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


