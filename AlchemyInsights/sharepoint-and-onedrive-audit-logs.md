---
title: Klassiska SharePoint-granskningsloggrapporter
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509618"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f11d3-102">Granskningsloggar för SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="f11d3-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f11d3-103">Klassiska granskningsloggar i SharePoint</span><span class="sxs-lookup"><span data-stu-id="f11d3-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f11d3-104">SPO:s äldre granskning migrerades till Unified Audit Log (UAL).</span><span class="sxs-lookup"><span data-stu-id="f11d3-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f11d3-105">Alla SPO-äldre granskningsrapporter kommer nu att drivas via UAL och de äldre granskningssignalerna har migrerats till UAL.</span><span class="sxs-lookup"><span data-stu-id="f11d3-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f11d3-106">Viktiga ändringar:</span><span class="sxs-lookup"><span data-stu-id="f11d3-106">Key changes:</span></span>

* <span data-ttu-id="f11d3-107">Trimning är INTE tillgänglig som en funktion.</span><span class="sxs-lookup"><span data-stu-id="f11d3-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f11d3-108">Att välja specifika händelser att granska är INTE tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="f11d3-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f11d3-109">Se [det här dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) för en fullständig lista över granskade händelser som är tillgängliga som standard.</span><span class="sxs-lookup"><span data-stu-id="f11d3-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f11d3-110">Alternativet **Plats** under **Anpassade rapporter** är INTE tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="f11d3-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f11d3-111">Alternativet **Öppna eller hämta dokumenthändelser** är INTE tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="f11d3-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f11d3-112">Konfigurera granskningsinställningar för en webbplatssamling</span><span class="sxs-lookup"><span data-stu-id="f11d3-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f11d3-113">SharePoint- och OneDrive-moderna enhetliga granskningsloggar från efterlevnad</span><span class="sxs-lookup"><span data-stu-id="f11d3-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f11d3-114">Aktivera/inaktivera enhetlig granskningsloggning</span><span class="sxs-lookup"><span data-stu-id="f11d3-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f11d3-115">Ingen ytterligare konfiguration krävs i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f11d3-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f11d3-116">Använd granskningsloggning för att kontrollera aktiviteten för filen eller mapparna, mapparna, användaren/kanna, behörigheterna:</span><span class="sxs-lookup"><span data-stu-id="f11d3-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f11d3-117">Fil- och sidaktiviteter</span><span class="sxs-lookup"><span data-stu-id="f11d3-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f11d3-118">Mappaktiviteter</span><span class="sxs-lookup"><span data-stu-id="f11d3-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f11d3-119">Aktiviteter för att dela och få åtkomst till begäran</span><span class="sxs-lookup"><span data-stu-id="f11d3-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f11d3-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="f11d3-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f11d3-121">Aktiviteter för webbplatsadministration</span><span class="sxs-lookup"><span data-stu-id="f11d3-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f11d3-122">Mer information om hur du hämtar dessa händelser finns i [Sök i granskningsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="f11d3-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
