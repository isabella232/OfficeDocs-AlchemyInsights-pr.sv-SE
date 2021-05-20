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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539842"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="4bd25-102">E-postmeddelanden saknas i karantän"</span><span class="sxs-lookup"><span data-stu-id="4bd25-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="4bd25-103">Administratörer kan [visa, släppa eller ta bort dessa meddelanden.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="4bd25-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="4bd25-104">Om du vill öppna & Säkerhets- och efterlevnadscenter går du till [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="4bd25-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="4bd25-105">Om du vill öppna sidan Karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="4bd25-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="4bd25-106">Du kan söka efter följande värden:</span><span class="sxs-lookup"><span data-stu-id="4bd25-106">You can search by the following values:</span></span>  

- <span data-ttu-id="4bd25-107">**Meddelande-ID**: Meddelandets globalt unika identifierare.</span><span class="sxs-lookup"><span data-stu-id="4bd25-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="4bd25-108">Om du markerar ett meddelande i listan visas värdet  **för Meddelande-ID**  i  **den**  utfällade rutan Information som visas.</span><span class="sxs-lookup"><span data-stu-id="4bd25-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="4bd25-109">Administratörer kan använda [meddelandespårning](/microsoft-365/security/office-365-security/message-trace-scc) för att söka efter meddelanden med motsvarande värden för meddelande-ID.</span><span class="sxs-lookup"><span data-stu-id="4bd25-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="4bd25-110">**Avsändarens e-postadress**: En enskild avsändarens e-postadress.</span><span class="sxs-lookup"><span data-stu-id="4bd25-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="4bd25-111">**Mottagarens e-postadress**: En enskild mottagares e-postadress.</span><span class="sxs-lookup"><span data-stu-id="4bd25-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="4bd25-112">**Ämne**: Använd meddelandets hela ämne.</span><span class="sxs-lookup"><span data-stu-id="4bd25-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="4bd25-113">Sökningen är inte skiftlägeskänslig.</span><span class="sxs-lookup"><span data-stu-id="4bd25-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="4bd25-114">När du har angett sökvillkor klickar du på ![knappen Uppdatera](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Uppdatera**, så filtreras resultatet.</span><span class="sxs-lookup"><span data-stu-id="4bd25-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="4bd25-115">De cmdlets du använder för att visa och hantera meddelanden och filer i karantän är:</span><span class="sxs-lookup"><span data-stu-id="4bd25-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="4bd25-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4bd25-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="4bd25-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4bd25-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="4bd25-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4bd25-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="4bd25-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Observera att den här cmdleten endast används för meddelanden, inte för skadlig programvara från Microsoft Defender för Office 365 för SharePoint Online, OneDrive för företag och Teams.</span><span class="sxs-lookup"><span data-stu-id="4bd25-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="4bd25-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="4bd25-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)