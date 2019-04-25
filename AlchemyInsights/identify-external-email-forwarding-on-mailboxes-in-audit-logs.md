---
title: Identifiera externa e-vidarebefordran på postlådor i granskningsloggar
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417229"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="3afcc-102">Identifiera när externa e-vidarebefordran har konfigurerats på postlådor</span><span class="sxs-lookup"><span data-stu-id="3afcc-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="3afcc-103">När en användare konfigurerar externa e-vidarebefordring på en postlåda, granskade aktiviteten som en del av cmdlet **Set-postlåda** .</span><span class="sxs-lookup"><span data-stu-id="3afcc-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="3afcc-104">Du kan se aktiviteten med Granska loggen Sök i säkerhet & regelefterlevnadscentret.</span><span class="sxs-lookup"><span data-stu-id="3afcc-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="3afcc-105">Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="3afcc-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="3afcc-106">Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.</span><span class="sxs-lookup"><span data-stu-id="3afcc-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="3afcc-107">Välj datumintervall i fälten **startdatum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="3afcc-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="3afcc-108">Du behöver inte ange ett användarnamn.</span><span class="sxs-lookup"><span data-stu-id="3afcc-108">You don't need to specify a username.</span></span> <span data-ttu-id="3afcc-109">Kontrollera fältet **verksamhet** är att **Visa resultat för alla aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="3afcc-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="3afcc-110">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="3afcc-110">Click **Search**.</span></span>

<span data-ttu-id="3afcc-111">I resultaten klickar du på **Filtrera resultat** och skriv **Set-postlåda** i filterrutan aktivitet.</span><span class="sxs-lookup"><span data-stu-id="3afcc-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="3afcc-112">Markera en granskningspost i resultaten.</span><span class="sxs-lookup"><span data-stu-id="3afcc-112">Select an audit record in the results.</span></span> <span data-ttu-id="3afcc-113">Klicka på **Mer information**i **information** -utfällbar.</span><span class="sxs-lookup"><span data-stu-id="3afcc-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="3afcc-114">Du behöver titta på detaljerna i varje Granskningspost för att avgöra om aktiviteten är relaterad till e-post vidarebefordras.</span><span class="sxs-lookup"><span data-stu-id="3afcc-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="3afcc-115">**Objekt-ID**: alias värdet för postlådan som ändrades.</span><span class="sxs-lookup"><span data-stu-id="3afcc-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="3afcc-116">**Parametrar**: _ForwardingSmtpAddress_ anger den e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="3afcc-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="3afcc-117">**Användar-ID**: den användare som konfigurerats för vidarebefordring av e-post på postlådan i fältet **objekt-ID** .</span><span class="sxs-lookup"><span data-stu-id="3afcc-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="3afcc-118">Mer information finns i [fastställa som definierar e-vidarebefordran för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="3afcc-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
