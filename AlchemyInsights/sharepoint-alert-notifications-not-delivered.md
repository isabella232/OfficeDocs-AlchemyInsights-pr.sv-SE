---
title: Aviseringar om SharePoint-aviseringar har inte levererats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742065"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="90cb4-102">Aviseringar om SharePoint-aviseringar har inte levererats</span><span class="sxs-lookup"><span data-stu-id="90cb4-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="90cb4-103">Kontrollera SKRÄP-mappen i din e-post, eftersom varningar ibland kan gå dit.</span><span class="sxs-lookup"><span data-stu-id="90cb4-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="90cb4-104">Ta reda på om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.</span><span class="sxs-lookup"><span data-stu-id="90cb4-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="90cb4-105">**Enskilda aviseringar levereras inte**: Om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den.</span><span class="sxs-lookup"><span data-stu-id="90cb4-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="90cb4-106">Se [Hantera, visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.</span><span class="sxs-lookup"><span data-stu-id="90cb4-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="90cb4-107">**Alla aviseringar levereras inte:** Om alla aviseringar från flera filer eller bibliotek inte levereras besöker du [instrumentpanelen för tjänstens hälsotillstånd](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att kontrollera om det finns några råd/incidenter som kan inträffa med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="90cb4-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="90cb4-108">Problemet kan vara med SharePoint-varningsfunktionen eller fördröjningar i e-postmeddelanden via Exchange.</span><span class="sxs-lookup"><span data-stu-id="90cb4-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="90cb4-109">Det kommer också att vara viktigt att notera om andra e-postmeddelanden levereras, och om inte, är problemet sannolikt med Exchange förseningar.</span><span class="sxs-lookup"><span data-stu-id="90cb4-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="90cb4-110">Vanliga frågor och svar om varningar:</span><span class="sxs-lookup"><span data-stu-id="90cb4-110">FAQ on alerts:</span></span>

- <span data-ttu-id="90cb4-111">Det går inte att skicka aviseringar till distributionsgrupp, endast säkerhets- och O365-grupper stöds.</span><span class="sxs-lookup"><span data-stu-id="90cb4-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="90cb4-112">Du kan inte anpassa aviseringsmallar för e-post. Du måste använda Microsoft FLOW eller SharePoint Designer Workflow för att uppnå dessa.</span><span class="sxs-lookup"><span data-stu-id="90cb4-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="90cb4-113">Mer information:</span><span class="sxs-lookup"><span data-stu-id="90cb4-113">More Information:</span></span>

- <span data-ttu-id="90cb4-114">**Aviseringsinställning:** Mer information om hur du konfigurerar aviseringar finns i [Skapa en avisering för att få ett meddelande när en fil eller mapp ändras i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="90cb4-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="90cb4-115">**Felsöka aviseringar:** Mer information om felsökningsaviseringar finns i [Användare får inte Aviseringar om SharePoint Online.](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)</span><span class="sxs-lookup"><span data-stu-id="90cb4-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="90cb4-116">**Avancerade principer för efterlevnad av O365:** Mer information om hur du konfigurerar dessa aviseringar finns i [principer för efterlevnadsvarning](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="90cb4-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="90cb4-117">**SharePoint- och OneDrive-granskningsloggar**: Mer information om hur du hämtar dessa händelser finns [i Sök i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="90cb4-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="90cb4-118">**Varningar som skickas av Avancerat skydd mot hot:** Se [ATP för SharePoint och OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="90cb4-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="90cb4-119">**Aviseringar som skickas av dataförlustförebyggande policyer:** Se [E-postmeddelanden för DLP-principer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="90cb4-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="90cb4-120">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="90cb4-120">Related Topics</span></span>

<span data-ttu-id="90cb4-121">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="90cb4-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="90cb4-122">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="90cb4-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="90cb4-123">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="90cb4-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
