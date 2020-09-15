---
title: Identifiera händelser för ta bort meddelanden i gransknings loggar
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696531"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="c1696-102">Gransknings loggar för borttagna e-postmeddelanden</span><span class="sxs-lookup"><span data-stu-id="c1696-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="c1696-103">Från och med den 2019 januari aktiverar Microsoft automatiskt gransknings loggning för post låda.</span><span class="sxs-lookup"><span data-stu-id="c1696-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="c1696-104">Om du till exempel vill ta bort meddelande händelser för en viss användare måste du manuellt aktivera borttagnings åtgärderna för granskning.</span><span class="sxs-lookup"><span data-stu-id="c1696-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="c1696-105">Om gransknings loggning för post lådor är aktiverat för din organisation eller för en viss användare följer du stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="c1696-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="c1696-106">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c1696-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c1696-107">Klicka på **Sök och** granska och välj **gransknings loggs ökning**.</span><span class="sxs-lookup"><span data-stu-id="c1696-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c1696-108">Välj datum intervall i fälten **start datum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="c1696-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c1696-109">Ange användar namn för den användare som du vill undersöka (användaren som tog bort objekten).</span><span class="sxs-lookup"><span data-stu-id="c1696-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="c1696-110">I fältet **aktiviteter** väljer du **borttagna meddelanden från mappen Borttaget** och **flyttade meddelanden till mappen Borttaget**.</span><span class="sxs-lookup"><span data-stu-id="c1696-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="c1696-111">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="c1696-111">Click **Search**.</span></span>

<span data-ttu-id="c1696-112">Välj en gransknings post i resultatet.</span><span class="sxs-lookup"><span data-stu-id="c1696-112">In the results, select an audit record.</span></span> <span data-ttu-id="c1696-113">I den utfällbara informationen klickar du på **Mer information**.</span><span class="sxs-lookup"><span data-stu-id="c1696-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c1696-114">Ytterligare information om det borttagna objektet (till exempel raden ämne och platsen för objektet när det togs bort) visas i fältet **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="c1696-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="c1696-115">Egenskapen **ClientInfoString** visar om borttagningen skedde i Outlook, Outlook på webben (tidigare Outlook Web App) eller annan enhet.</span><span class="sxs-lookup"><span data-stu-id="c1696-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="c1696-116">Mer information finns i [bestämma vem som konfigurerar e-postvidarebefordran för en post låda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="c1696-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="c1696-117">**Obs!** du kan inte hämta borttagna objekt med hjälp av Gransknings logg funktionen.</span><span class="sxs-lookup"><span data-stu-id="c1696-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="c1696-118">Information om hur du hämtar borttagna meddelanden i Outlook på webben finns i [återställa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="c1696-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
