---
title: E-postmeddelanden som saknas i karantän
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673732"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="b12b3-102">E-postmeddelanden som saknas i karantän "</span><span class="sxs-lookup"><span data-stu-id="b12b3-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="b12b3-103">Administratörer kan [Visa, frigöra eller ta bort dessa meddelanden.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="b12b3-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="b12b3-104">Om du vill öppna säkerhets & Compliance Center går du till [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="b12b3-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="b12b3-105">Om du vill öppna sidan karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="b12b3-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="b12b3-106">Du kan söka efter följande värden:</span><span class="sxs-lookup"><span data-stu-id="b12b3-106">You can search by the following values:</span></span>  

- <span data-ttu-id="b12b3-107">**Meddelande-ID**: Meddelandets globalt unika identifierare.</span><span class="sxs-lookup"><span data-stu-id="b12b3-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="b12b3-108">Om du väljer ett meddelande i listan visas värdet för  **meddelande-ID**  i fönstret  **detaljerad information**  .</span><span class="sxs-lookup"><span data-stu-id="b12b3-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="b12b3-109">Administratörer kan använda [meddelandespårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) för att söka efter meddelanden med motsvarande värden för meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="b12b3-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="b12b3-110">**Avsändarens e-postadress**: En enskild avsändarens e-postadress.</span><span class="sxs-lookup"><span data-stu-id="b12b3-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="b12b3-111">**Mottagarens e-postadress**: En enskild mottagares e-postadress.</span><span class="sxs-lookup"><span data-stu-id="b12b3-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="b12b3-112">**Ämne**: Använd meddelandets hela ämne.</span><span class="sxs-lookup"><span data-stu-id="b12b3-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="b12b3-113">Sökningen är inte skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="b12b3-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="b12b3-114">När du har angett Sök villkoren klickar du på ![ uppdatera knappen uppdatera ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** för att filtrera resultaten.  </span><span class="sxs-lookup"><span data-stu-id="b12b3-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="b12b3-115">De cmdlets som du använder för att visa och hantera meddelanden och filer i karantänen är:</span><span class="sxs-lookup"><span data-stu-id="b12b3-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="b12b3-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b12b3-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="b12b3-117">Exportera-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b12b3-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="b12b3-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b12b3-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="b12b3-119">För [hands version – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Observera att denna cmdlet endast gäller för meddelanden, inte malware-filer från ATP för SharePoint Online, OneDrive för företag eller teams.</span><span class="sxs-lookup"><span data-stu-id="b12b3-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="b12b3-120">Utgivning-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="b12b3-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)