---
title: Klassiska SharePoint-granskningsloggrapporter
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068041"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="a734d-102">Granskningsloggar för SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="a734d-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="a734d-103">**SharePoint och OneDrive moderna enhetliga granskningsloggar från efterlevnad**</span><span class="sxs-lookup"><span data-stu-id="a734d-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="a734d-104">Aktivera/inaktivera enhetlig granskningsloggning</span><span class="sxs-lookup"><span data-stu-id="a734d-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="a734d-105">Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a734d-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="a734d-106">Använd granskningsloggning Sök för att kontrollera aktiviteten för filen (s), mapp (ar), användare (s), behörigheter:</span><span class="sxs-lookup"><span data-stu-id="a734d-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="a734d-107">Fil-och sid aktiviteter</span><span class="sxs-lookup"><span data-stu-id="a734d-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="a734d-108">Mappaktiviteter</span><span class="sxs-lookup"><span data-stu-id="a734d-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="a734d-109">Aktiviteter för delning och åtkomstbegäran</span><span class="sxs-lookup"><span data-stu-id="a734d-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="a734d-110">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="a734d-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="a734d-111">Aktiviteter för Webbplatsadministration</span><span class="sxs-lookup"><span data-stu-id="a734d-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="a734d-112">Mer information om hur du hämtar dessa händelser finns [i söka i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="a734d-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="a734d-113">**Klassiska SharePoint-granskningsloggar**</span><span class="sxs-lookup"><span data-stu-id="a734d-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="a734d-114">Vi migrerade SPO Legacy Auditing till Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="a734d-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="a734d-115">Detta innebär i huvudsak att alla SPO äldre granskningsrapporter nu kommer att drivas via UAL och att de äldre gransknings signalerna har migrerats till UAL.</span><span class="sxs-lookup"><span data-stu-id="a734d-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="a734d-116">Viktiga ändringar:</span><span class="sxs-lookup"><span data-stu-id="a734d-116">Key changes:</span></span>

- <span data-ttu-id="a734d-117">Trimning som en funktion är inte tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="a734d-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="a734d-118">Avsnittet där du väljer specifika händelser för granskning är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="a734d-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="a734d-119">Se [detta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.</span><span class="sxs-lookup"><span data-stu-id="a734d-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="a734d-120">Alternativet "plats" under **anpassade rapporter** är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="a734d-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="a734d-121">"Öppna eller ladda ned dokument" händelser är inte tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="a734d-121">“Opening or downloading documents” events is NOT available.</span></span> 

