---
title: Identifiera extern vidarebefordran av e-post i post lådor i gransknings loggar
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696315"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="2f594-102">Identifiera när extern e-postvidarebefordran är konfigurerad på post lådor</span><span class="sxs-lookup"><span data-stu-id="2f594-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="2f594-103">När en Microsoft 365-användare konfigurerar extern e-postvidarebefordran i en post låda granskas aktiviteten som en del av cmdleten **set-post låda** .</span><span class="sxs-lookup"><span data-stu-id="2f594-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="2f594-104">Du kan se aktiviteten med hjälp av gransknings loggs ökning i centret för säkerhets & efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="2f594-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="2f594-105">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2f594-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2f594-106">Gå till sidan **Sök**  >  **gransknings loggs sökning** .</span><span class="sxs-lookup"><span data-stu-id="2f594-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2f594-107">Välj datum intervall i fälten **start datum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="2f594-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="2f594-108">Du behöver inte ange ett användar namn.</span><span class="sxs-lookup"><span data-stu-id="2f594-108">You don't need to specify a username.</span></span> <span data-ttu-id="2f594-109">Kontrol lera att fältet **aktiviteter** är inställt på **Visa resultat för alla aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="2f594-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="2f594-110">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="2f594-110">Click **Search**.</span></span>

<span data-ttu-id="2f594-111">Klicka på **filter resultat** och skriv **in post låda** i rutan aktivitets filter.</span><span class="sxs-lookup"><span data-stu-id="2f594-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="2f594-112">Välj en gransknings post i resultatet.</span><span class="sxs-lookup"><span data-stu-id="2f594-112">Select an audit record in the results.</span></span> <span data-ttu-id="2f594-113">I den utfällbara **informationen** klickar du på **Mer information**.</span><span class="sxs-lookup"><span data-stu-id="2f594-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="2f594-114">Du måste granska detaljerna för varje gransknings post för att avgöra om aktiviteten är relaterad till vidarebefordran via e-post.</span><span class="sxs-lookup"><span data-stu-id="2f594-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="2f594-115">**ObjectID**: Ali Aset för post lådan som har ändrats.</span><span class="sxs-lookup"><span data-stu-id="2f594-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="2f594-116">**Parametrar**: _ForwardingSmtpAddress_ anger mål-e-postadress.</span><span class="sxs-lookup"><span data-stu-id="2f594-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="2f594-117">**UserID**: användaren som konfigurerade e-postvidarebefordran på post lådan i fältet **ObjectID** .</span><span class="sxs-lookup"><span data-stu-id="2f594-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="2f594-118">Mer information finns i [bestämma vem som konfigurerar e-postvidarebefordran för en post låda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="2f594-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
