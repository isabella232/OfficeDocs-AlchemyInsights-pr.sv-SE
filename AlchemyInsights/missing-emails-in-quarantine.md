---
title: E-postmeddelanden saknas i karantän
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831752"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="89b98-102">E-postmeddelanden saknas i karantän"</span><span class="sxs-lookup"><span data-stu-id="89b98-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="89b98-103">Administratörer kan [visa, släppa eller ta bort dessa meddelanden.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="89b98-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="89b98-104">Om du vill öppna & Säkerhets- och efterlevnadscenter går du till [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="89b98-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="89b98-105">Om du vill öppna sidan Karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="89b98-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="89b98-106">Du kan söka efter följande värden:</span><span class="sxs-lookup"><span data-stu-id="89b98-106">You can search by the following values:</span></span>  

- <span data-ttu-id="89b98-107">**Meddelande-ID**: Meddelandets globalt unika identifierare.</span><span class="sxs-lookup"><span data-stu-id="89b98-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="89b98-108">Om du markerar ett meddelande i listan visas värdet  **för Meddelande-ID**  i  **den**  utfällade rutan Information som visas.</span><span class="sxs-lookup"><span data-stu-id="89b98-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="89b98-109">Administratörer kan använda [meddelandespårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) för att söka efter meddelanden med motsvarande värden för meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="89b98-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="89b98-110">**Avsändarens e-postadress**: En enskild avsändarens e-postadress.</span><span class="sxs-lookup"><span data-stu-id="89b98-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="89b98-111">**Mottagarens e-postadress**: En enskild mottagares e-postadress.</span><span class="sxs-lookup"><span data-stu-id="89b98-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="89b98-112">**Ämne**: Använd meddelandets hela ämne.</span><span class="sxs-lookup"><span data-stu-id="89b98-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="89b98-113">Sökningen är inte skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="89b98-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="89b98-114">När du har angett sökvillkoren klickar du på ![ Uppdatera knappen Uppdatera ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **för** att filtrera resultatet.  </span><span class="sxs-lookup"><span data-stu-id="89b98-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="89b98-115">De cmdlets du använder för att visa och hantera meddelanden och filer i karantän är:</span><span class="sxs-lookup"><span data-stu-id="89b98-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="89b98-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="89b98-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="89b98-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="89b98-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="89b98-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="89b98-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="89b98-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Observera att den här cmdleten endast används för meddelanden, inte för skadlig programvara från ATP för SharePoint Online, OneDrive för företag eller Teams.</span><span class="sxs-lookup"><span data-stu-id="89b98-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="89b98-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="89b98-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)