---
title: Identifiera borttagning av meddelandehändelser i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509006"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="11e5b-102">Granskningsloggar för borttagna e-postmeddelanden</span><span class="sxs-lookup"><span data-stu-id="11e5b-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="11e5b-103">Från och med januari 2019 aktiverar Microsoft loggning av postlådor som standard.</span><span class="sxs-lookup"><span data-stu-id="11e5b-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="11e5b-104">Om du vill granska borttagningshändelser för en viss användare måste du aktivera borttagningsåtgärderna manuellt för granskning.</span><span class="sxs-lookup"><span data-stu-id="11e5b-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="11e5b-105">Om loggning av postlådor redan är aktiverat för din organisation eller för den specifika användaren följer du stegen nedan.</span><span class="sxs-lookup"><span data-stu-id="11e5b-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="11e5b-106">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="11e5b-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="11e5b-107">Klicka på **Sök och utredning** och välj **Granskningsloggsökning**.</span><span class="sxs-lookup"><span data-stu-id="11e5b-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="11e5b-108">Välj datumintervall i fälten **Startdatum** och **Slutdatum.**</span><span class="sxs-lookup"><span data-stu-id="11e5b-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="11e5b-109">Ange användarnamn för den användare som du vill undersöka (användaren som tog bort objekten).</span><span class="sxs-lookup"><span data-stu-id="11e5b-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="11e5b-110">I fältet **Aktiviteter** väljer du **Borttagna meddelanden från mappen Borttaget** och **Flyttade meddelanden till mappen Borttaget.**</span><span class="sxs-lookup"><span data-stu-id="11e5b-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="11e5b-111">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="11e5b-111">Click **Search**.</span></span>

<span data-ttu-id="11e5b-112">Välj en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="11e5b-112">In the results, select an audit record.</span></span> <span data-ttu-id="11e5b-113">Klicka på **Mer information**i informationsutfällbara.</span><span class="sxs-lookup"><span data-stu-id="11e5b-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="11e5b-114">Ytterligare information om det borttagna objektet (till exempel ämnesraden och platsen för objektet när det togs bort) visas i fältet **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="11e5b-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="11e5b-115">Egenskapen **ClientInfoString** visas om borttagningen inträffade i Outlook, Outlook på webben (tidigare kallat Outlook Web App) eller någon annan enhet.</span><span class="sxs-lookup"><span data-stu-id="11e5b-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="11e5b-116">Mer information finns i [Bestämma vem som konfigurerar vidarebefordran av e-post för en postlåda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="11e5b-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="11e5b-117">**Du**kan inte hämta borttagna objekt med hjälp av granskningsloggfunktionen.</span><span class="sxs-lookup"><span data-stu-id="11e5b-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="11e5b-118">Information om hur du hämtar borttagna meddelanden i Outlook på webben finns [i Återställa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="11e5b-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
