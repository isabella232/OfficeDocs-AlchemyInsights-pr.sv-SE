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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992636"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="8cfd5-102">Granskningsloggar för SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="8cfd5-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="8cfd5-103">Klassiska SharePoint-granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="8cfd5-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="8cfd5-104">SPO Legacy Auditing migrerades till Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="8cfd5-105">Alla SPO äldre granskningsrapporter kommer nu att drivas via UAL och de äldre gransknings signalerna har migrerats till UAL.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="8cfd5-106">Viktiga ändringar:</span><span class="sxs-lookup"><span data-stu-id="8cfd5-106">Key changes:</span></span>

* <span data-ttu-id="8cfd5-107">Trimning är inte tillgänglig som en funktion.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="8cfd5-108">Det går inte att välja specifika händelser för granskning.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="8cfd5-109">Se [detta dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="8cfd5-110">Alternativet **plats** under **anpassade rapporter** är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="8cfd5-111">Alternativet **Öppna eller hämta dokument** händelser är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="8cfd5-112">Konfigurera granskningsinställningar för en webbplatssamling</span><span class="sxs-lookup"><span data-stu-id="8cfd5-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="8cfd5-113">SharePoint och OneDrive moderna enhetliga granskningsloggar från efterlevnad</span><span class="sxs-lookup"><span data-stu-id="8cfd5-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="8cfd5-114">Aktivera/inaktivera enhetlig granskningsloggning</span><span class="sxs-lookup"><span data-stu-id="8cfd5-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="8cfd5-115">Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8cfd5-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="8cfd5-116">Använd granskningsloggning Sök för att kontrollera aktiviteten för filen (s), mapp (ar), användare (s), behörigheter:</span><span class="sxs-lookup"><span data-stu-id="8cfd5-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="8cfd5-117">Fil-och sid aktiviteter</span><span class="sxs-lookup"><span data-stu-id="8cfd5-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="8cfd5-118">Mappaktiviteter</span><span class="sxs-lookup"><span data-stu-id="8cfd5-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="8cfd5-119">Aktiviteter för delning och åtkomstbegäran</span><span class="sxs-lookup"><span data-stu-id="8cfd5-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="8cfd5-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="8cfd5-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="8cfd5-121">Aktiviteter för Webbplatsadministration</span><span class="sxs-lookup"><span data-stu-id="8cfd5-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="8cfd5-122">Mer information om hur du hämtar dessa händelser finns [i söka i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="8cfd5-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
