---
title: Identifiera extern vidarebefordran av e-post på postlådor i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508970"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="a9a16-102">Identifiera när extern vidarebefordran av e-post är konfigurerad på postlådor</span><span class="sxs-lookup"><span data-stu-id="a9a16-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="a9a16-103">När en Microsoft 365-användare konfigurerar extern vidarebefordran av e-post på en postlåda granskas aktiviteten som en del av cmdleten **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="a9a16-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="a9a16-104">Du kan se aktiviteten med hjälp av granskningsloggsökning i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="a9a16-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="a9a16-105">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a9a16-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a9a16-106">Gå till söksidan **för sökfunktionen i**  >  **sökgranskning.**</span><span class="sxs-lookup"><span data-stu-id="a9a16-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="a9a16-107">Välj datumintervall i fälten **Startdatum** och **Slutdatum.**</span><span class="sxs-lookup"><span data-stu-id="a9a16-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a9a16-108">Du behöver inte ange ett användarnamn.</span><span class="sxs-lookup"><span data-stu-id="a9a16-108">You don't need to specify a username.</span></span> <span data-ttu-id="a9a16-109">Kontrollera att fältet **Aktiviteter** är inställt på **Visa resultat för alla aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="a9a16-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="a9a16-110">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="a9a16-110">Click **Search**.</span></span>

<span data-ttu-id="a9a16-111">I resultatet klickar du på **Filtrera resultat** och skriver **Set-Postlåda** i rutan aktivitetsfilter.</span><span class="sxs-lookup"><span data-stu-id="a9a16-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="a9a16-112">Välj en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="a9a16-112">Select an audit record in the results.</span></span> <span data-ttu-id="a9a16-113">Klicka på **Mer information**i utfällbara **information.**</span><span class="sxs-lookup"><span data-stu-id="a9a16-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="a9a16-114">Du måste titta på information om varje granskningspost för att avgöra om aktiviteten är relaterad till vidarebefordran av e-post.</span><span class="sxs-lookup"><span data-stu-id="a9a16-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="a9a16-115">**ObjectId**: Aliasvärdet för postlådan som har ändrats.</span><span class="sxs-lookup"><span data-stu-id="a9a16-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="a9a16-116">**Parametrar**: _ForwardingSmtpAddress_ anger målet e-postadress.</span><span class="sxs-lookup"><span data-stu-id="a9a16-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="a9a16-117">**UserId**: Användaren som konfigurerade vidarebefordran av e-post på postlådan i fältet **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="a9a16-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="a9a16-118">Mer information finns i [Bestämma vem som konfigurerar vidarebefordran av e-post för en postlåda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a9a16-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
