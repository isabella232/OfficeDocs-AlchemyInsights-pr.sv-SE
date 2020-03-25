---
title: DLP-principtips fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932604"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="814e1-102">Problem med DLP-principtips</span><span class="sxs-lookup"><span data-stu-id="814e1-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="814e1-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="814e1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="814e1-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="814e1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="814e1-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="814e1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="814e1-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="814e1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="814e1-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="814e1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="814e1-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="814e1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="814e1-109">**Tips för DLP-policy**</span><span class="sxs-lookup"><span data-stu-id="814e1-109">**DLP policy tips**</span></span>

<span data-ttu-id="814e1-110">När du använder **DLP-principer**kan användare meddelas om en policyöverträdelse med **principtips**.</span><span class="sxs-lookup"><span data-stu-id="814e1-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="814e1-111">Administratörer kan konfigurera principtips som ska visas när de testar sin DLP-princip eller när principen är i fullständigt tvingande läge.</span><span class="sxs-lookup"><span data-stu-id="814e1-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="814e1-112">Så här konfigurerar du principtips för DLP-principen i säkerhets- och efterlevnadscentret i fullständigt tvingande läge:</span><span class="sxs-lookup"><span data-stu-id="814e1-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="814e1-113">Kontrollera att principtips har **aktiverats** på DLP-regeln med hjälp av stegen [här](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="814e1-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="814e1-114">Se till att **ditt innehåll matchar** vad som **krävs** för att utlösa regeln som beskrivs i den här artikeln [här](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="814e1-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="814e1-115">Principtips visas i både OWA och Outlook.</span><span class="sxs-lookup"><span data-stu-id="814e1-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="814e1-116">När du använder **Outlook 2013 eller senare**visas dock principtips endast under vissa förhållanden.</span><span class="sxs-lookup"><span data-stu-id="814e1-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="814e1-117">Dessa villkor visas här: [Villkor som stöds för Outlook 2013 eller senare för att visa principtips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="814e1-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="814e1-118">Mer information om DLP-principtips finns i: [Visa principtips för DLP-principer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="814e1-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  