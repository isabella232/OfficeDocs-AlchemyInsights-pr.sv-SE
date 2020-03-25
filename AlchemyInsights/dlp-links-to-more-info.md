---
title: Mer information om DLP-problem
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932712"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="bda85-102">Information om DLP-problem</span><span class="sxs-lookup"><span data-stu-id="bda85-102">Information about DLP issues</span></span>

<span data-ttu-id="bda85-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="bda85-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="bda85-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="bda85-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="bda85-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="bda85-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="bda85-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="bda85-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="bda85-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="bda85-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="bda85-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="bda85-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="bda85-109">**Information om DLP-principen**</span><span class="sxs-lookup"><span data-stu-id="bda85-109">**Information on DLP policy**</span></span>

<span data-ttu-id="bda85-110">Med en DLP-princip kan du identifiera, övervaka och automatiskt skydda känslig information i Office 365.</span><span class="sxs-lookup"><span data-stu-id="bda85-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="bda85-111">Besök dessa länkar för mer information:</span><span class="sxs-lookup"><span data-stu-id="bda85-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="bda85-112">Översikt över dataförlustskydd</span><span class="sxs-lookup"><span data-stu-id="bda85-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="bda85-113">Vad de känsliga informationstyperna letar efter</span><span class="sxs-lookup"><span data-stu-id="bda85-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="bda85-114">Skapa en anpassad känslig informationstyp</span><span class="sxs-lookup"><span data-stu-id="bda85-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="bda85-115">Skicka e-postmeddelanden och visa policytips</span><span class="sxs-lookup"><span data-stu-id="bda85-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="bda85-116">Skydda SharePoint Online-filer med kvarhållningsetiketter och DLP</span><span class="sxs-lookup"><span data-stu-id="bda85-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="bda85-117">DLP och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bda85-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="bda85-118">Om du vill testa dina data med en inbyggd eller anpassad känslig informationstyp använder du alternativet **Testtyp** under Klassificeringar känsliga **informationstyper** > **Sensitive info types**.</span><span class="sxs-lookup"><span data-stu-id="bda85-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="bda85-119">Mer information finns i [Testa anpassade typer av känslig information](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="bda85-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>