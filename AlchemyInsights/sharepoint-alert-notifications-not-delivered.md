---
title: SharePoint-aviseringarna har inte levererats
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744659"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="db931-102">SharePoint-aviseringarna har inte levererats</span><span class="sxs-lookup"><span data-stu-id="db931-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="db931-103">Vänligen kontrollera skräppostmappen i din e-post, eftersom ibland kan varningar gå dit.</span><span class="sxs-lookup"><span data-stu-id="db931-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="db931-104">Ta reda på om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.</span><span class="sxs-lookup"><span data-stu-id="db931-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="db931-105">**Enskilda aviseringar levereras inte**: om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den.</span><span class="sxs-lookup"><span data-stu-id="db931-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="db931-106">Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) för att återskapa aviseringen.</span><span class="sxs-lookup"><span data-stu-id="db931-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="db931-107">**Alla aviseringar levereras inte**: om alla aviseringar från flera filer eller bibliotek inte levereras, gå till [instrumentpanelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att kontrollera om det finns några bulletiner/incidenter som kan inträffa med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="db931-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="db931-108">Problemet kan vara med SharePoint alert-funktionen eller fördröjningar i e-postmeddelanden via Exchange.</span><span class="sxs-lookup"><span data-stu-id="db931-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="db931-109">Det kommer också att vara viktigt att notera om andra e-post levereras, och om inte, är problemet sannolikt med Exchange förseningar.</span><span class="sxs-lookup"><span data-stu-id="db931-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="db931-110">FAQ om varningar:</span><span class="sxs-lookup"><span data-stu-id="db931-110">FAQ on alerts:</span></span>

- <span data-ttu-id="db931-111">Det går inte att skicka aviseringar till distributionsgruppen, endast säkerhets-och O365-grupper stöds.</span><span class="sxs-lookup"><span data-stu-id="db931-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="db931-112">Du kan inte anpassa e-postmallar för notifieringar. Du måste använda Microsoft FLOW eller SharePoint Designer arbetsflöde för att uppnå dessa.</span><span class="sxs-lookup"><span data-stu-id="db931-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="db931-113">Mer information:</span><span class="sxs-lookup"><span data-stu-id="db931-113">More Information:</span></span>

- <span data-ttu-id="db931-114">**Aviseringsinställning**: Mer information om hur du ställer in aviseringar finns [i skapa en avisering för att få ett meddelande när en fil eller mapp ändras i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="db931-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="db931-115">**Felsöka aviseringar**: Mer information om felsökning av aviseringar finns i [användare får inte SharePoint Online varningsmeddelanden](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="db931-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="db931-116">**Avancerad O365-efterlevnad varnings principer**: Mer information om hur du ställer in dessa aviseringar finns i [efterlevnad aviserings principer](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="db931-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="db931-117">**SharePoint och OneDrive granskningsloggar**: Mer information om hur du hämtar dessa händelser finns [i Sök i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="db931-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="db931-118">**Aviseringar som skickas av Advanced Threat Protection**: se [ATP för SharePoint och OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="db931-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="db931-119">**Aviseringar som skickas av data förlust förebyggande principer**: se [e-POSTAVISERINGAR för DLP-principer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="db931-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="db931-120">Närliggande ämnen</span><span class="sxs-lookup"><span data-stu-id="db931-120">Related Topics</span></span>

<span data-ttu-id="db931-121">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="db931-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="db931-122">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="db931-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="db931-123">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="db931-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
