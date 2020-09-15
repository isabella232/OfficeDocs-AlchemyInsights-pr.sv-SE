---
title: Klassiska redovisnings rapporter för SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662226"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="b01c0-102">Gransknings loggar för SharePoint och OneDrive</span><span class="sxs-lookup"><span data-stu-id="b01c0-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="b01c0-103">Klassiska SharePoint-gransknings loggar</span><span class="sxs-lookup"><span data-stu-id="b01c0-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="b01c0-104">SPO Legacy-granskning migrerades till Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="b01c0-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="b01c0-105">Alla SPO-gransknings rapporter kommer nu att startas med UAL och de äldre gransknings signalerna har migrerats till UAL.</span><span class="sxs-lookup"><span data-stu-id="b01c0-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="b01c0-106">Viktiga ändringar:</span><span class="sxs-lookup"><span data-stu-id="b01c0-106">Key changes:</span></span>

* <span data-ttu-id="b01c0-107">Trimning är inte tillgänglig som en funktion.</span><span class="sxs-lookup"><span data-stu-id="b01c0-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="b01c0-108">Det går inte att välja specifika händelser som ska granskas.</span><span class="sxs-lookup"><span data-stu-id="b01c0-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="b01c0-109">I [det här dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) finns en fullständig lista över granskade händelser som är tillgängliga som standard.</span><span class="sxs-lookup"><span data-stu-id="b01c0-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="b01c0-110">Alternativet **plats** under **anpassade rapporter** är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="b01c0-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="b01c0-111">Alternativet för att **Öppna eller ladda ned dokument** händelser är inte tillgängligt.</span><span class="sxs-lookup"><span data-stu-id="b01c0-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="b01c0-112">Konfigurera gransknings inställningar för en webbplats samling</span><span class="sxs-lookup"><span data-stu-id="b01c0-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="b01c0-113">SharePoint-och OneDrive-moderna enhetliga redovisnings loggar från efterlevnad</span><span class="sxs-lookup"><span data-stu-id="b01c0-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="b01c0-114">Aktivera/inaktivera enhetlig gransknings loggning</span><span class="sxs-lookup"><span data-stu-id="b01c0-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="b01c0-115">Det krävs ingen ytterligare konfiguration i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b01c0-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="b01c0-116">Använd gransknings loggnings sökning för att kontrol lera aktivitet för filer, mappar, användare, behörigheter:</span><span class="sxs-lookup"><span data-stu-id="b01c0-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="b01c0-117">Fil-och sid aktiviteter</span><span class="sxs-lookup"><span data-stu-id="b01c0-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="b01c0-118">Mappaktiviteter</span><span class="sxs-lookup"><span data-stu-id="b01c0-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="b01c0-119">Aktiviteter för delning och åtkomstbegäran</span><span class="sxs-lookup"><span data-stu-id="b01c0-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="b01c0-120">Synkroniseringsuppgift</span><span class="sxs-lookup"><span data-stu-id="b01c0-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="b01c0-121">Aktiviteter för webbplats administration</span><span class="sxs-lookup"><span data-stu-id="b01c0-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="b01c0-122">Mer information om hur du hämtar de här händelserna finns i [söka i gransknings loggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="b01c0-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
