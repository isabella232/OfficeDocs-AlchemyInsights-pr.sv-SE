---
title: Identifiera delete message händelser i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755170"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="c786f-102">Granska loggarna för borttagna e-postmeddelanden</span><span class="sxs-lookup"><span data-stu-id="c786f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="c786f-103">Börjar i januari 2019 Microsoft aktivera postlådan Granskningsloggningen som standard.</span><span class="sxs-lookup"><span data-stu-id="c786f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="c786f-104">Annars, om du vill granska händelser för ta bort meddelande för en viss användare, måste du aktivera manuellt ta bort åtgärder för granskning.</span><span class="sxs-lookup"><span data-stu-id="c786f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="c786f-105">Om postlådan granska loggning är redan aktiverat för organisationen eller för specifika användare, följer du stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="c786f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="c786f-106">Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c786f-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c786f-107">Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.</span><span class="sxs-lookup"><span data-stu-id="c786f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c786f-108">Välj datumintervall i fälten **startdatum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="c786f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c786f-109">Ange användarnamnet för den användare som du vill undersöka (användare som borttagna objekt).</span><span class="sxs-lookup"><span data-stu-id="c786f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="c786f-110">Välj i fältet **verksamhet** **borttagna meddelanden från mappen Borttaget** och **Moved meddelanden till mappen Borttaget**.</span><span class="sxs-lookup"><span data-stu-id="c786f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="c786f-111">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="c786f-111">Click **Search**.</span></span>

<span data-ttu-id="c786f-112">Markera en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="c786f-112">In the results, select an audit record.</span></span> <span data-ttu-id="c786f-113">Klicka på **Mer Information**i information-utfällbar.</span><span class="sxs-lookup"><span data-stu-id="c786f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c786f-114">Ytterligare information om det borttagna objektet (till exempel ämnesraden och placeringen av objektet när den togs bort) visas i fältet **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="c786f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="c786f-115">Egenskapen **ClientInfoString** visas om borttagningen uppstod i Outlook, Outlook på webben (kallades tidigare Outlook Web App) eller någon annan enhet.</span><span class="sxs-lookup"><span data-stu-id="c786f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="c786f-116">Mer information finns i [fastställa som definierar e-vidarebefordran för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="c786f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="c786f-117">**Obs**: du kan inte hämta borttagna objekt med hjälp av funktionen Granska loggen.</span><span class="sxs-lookup"><span data-stu-id="c786f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="c786f-118">Om du vill återställa borttagna meddelanden i Outlook på webben finns i [Återskapa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="c786f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
