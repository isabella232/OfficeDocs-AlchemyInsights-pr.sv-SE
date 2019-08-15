---
title: SharePoint-aviseringar inte levereras
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
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404820"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="d46c6-102">SharePoint-aviseringar inte levereras</span><span class="sxs-lookup"><span data-stu-id="d46c6-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="d46c6-103">Kontrollera mappen Skräppost i ditt e-postmeddelande som aviseringar kan ibland gå dit.</span><span class="sxs-lookup"><span data-stu-id="d46c6-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="d46c6-104">Ta reda på om **alla notifieringar inte levereras** eller om **ett enskilt meddelande** från en specifik fil eller biblioteket inte har levererats.</span><span class="sxs-lookup"><span data-stu-id="d46c6-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="d46c6-105">**Enskilda meddelanden levereras inte**: om en enskild avisering från en specifik fil eller biblioteket inte levereras, du kan försöka ta bort och återskapa den.</span><span class="sxs-lookup"><span data-stu-id="d46c6-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="d46c6-106">Se [Hantera, visa, eller ta bort avisering](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) att skapa aviseringen.</span><span class="sxs-lookup"><span data-stu-id="d46c6-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="d46c6-107">**Alla notifieringar inte levereras**: Besök [tjänsten hälsa instrumentpanelen](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för alla rekommendationerna/händelser som sker med SharePoint- eller om alla aviseringar från flera filer och bibliotek inte har levererats.</span><span class="sxs-lookup"><span data-stu-id="d46c6-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d46c6-108">Problemet kan bero på SharePoint alert kapacitet eller fördröjningar i e-postmeddelanden via Exchange.</span><span class="sxs-lookup"><span data-stu-id="d46c6-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d46c6-109">Det blir också viktigt att notera om annan e-post levereras och inte problemet sannolikt på förseningar i Exchange.</span><span class="sxs-lookup"><span data-stu-id="d46c6-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="d46c6-110">Vanliga frågor och svar om aviseringar:</span><span class="sxs-lookup"><span data-stu-id="d46c6-110">FAQ on alerts:</span></span>

- <span data-ttu-id="d46c6-111">Det är inte möjligt att skicka aviseringar till distributionsgruppen endast säkerhet och O365 grupper stöds.</span><span class="sxs-lookup"><span data-stu-id="d46c6-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="d46c6-112">Du kan inte anpassa alert e-mallar. Du måste använda Microsoft FLOW eller arbetsflödet i SharePoint Designer för att uppnå de.</span><span class="sxs-lookup"><span data-stu-id="d46c6-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="d46c6-113">Mer Information:</span><span class="sxs-lookup"><span data-stu-id="d46c6-113">More Information:</span></span>

- <span data-ttu-id="d46c6-114">**Notifieringsinställningar**: Mer information om hur du ställer in notifieringar finns i [Skapa en avisering om du vill bli meddelad när en fil eller mapp ändras i SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="d46c6-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="d46c6-115">**Felsöka varningar**: Mer information om felsökning av meddelanden finns i [användare får inte SharePoint Online aviseringar](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="d46c6-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="d46c6-116">**Avancerade O365 överensstämmelse Alert principer**: Mer information om hur du konfigurerar dessa aviseringar finns i [Alert principer för överensstämmelse](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="d46c6-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="d46c6-117">**SharePoint och OneDrive granska loggar**: Mer information om hur du hämtar dessa händelser finns i [söka granskningsloggen](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d46c6-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="d46c6-118">**Meddelanden som skickas av Advanced Threat Protection**: finns [tillgängligt att LOVA för SharePoint och OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d46c6-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="d46c6-119">**Principer för notifieringar som skickas av förhindra dataförlust**: se [e-postmeddelanden för DLP-principer](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="d46c6-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d46c6-120">Närliggande information</span><span class="sxs-lookup"><span data-stu-id="d46c6-120">Related Topics</span></span>

<span data-ttu-id="d46c6-121">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="d46c6-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="d46c6-122">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="d46c6-122">Create Flow</span></span>](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="d46c6-123">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="d46c6-123">SharePoint and Flow</span></span>](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
