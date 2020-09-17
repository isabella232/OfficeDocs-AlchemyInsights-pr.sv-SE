---
title: Återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799222"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="bb78c-102">Återkalla eller ersätta ett e-postmeddelande i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bb78c-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="bb78c-103">Du kan **bara återkalla meddelanden som skickas till personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="bb78c-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="bb78c-104">Om meddelandet skickades till en Gmail-adress, till exempel, kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="bb78c-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="bb78c-105">Du kan **bara återkalla meddelanden som skickats från Outlook 2016 för PC**.</span><span class="sxs-lookup"><span data-stu-id="bb78c-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="bb78c-106">Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="bb78c-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="bb78c-107">Om du är administratör kan du **återkalla meddelanden för användare med hjälp av PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="bb78c-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="bb78c-108">Du kan inte återkalla meddelanden från administrations centret.</span><span class="sxs-lookup"><span data-stu-id="bb78c-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="bb78c-109">Bläddra ned till "Sök efter och ta bort e-postmeddelanden i din organisation" för mer information.</span><span class="sxs-lookup"><span data-stu-id="bb78c-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="bb78c-110">**Återkalla eller ersätta ett e-postmeddelande som du har skickat**</span><span class="sxs-lookup"><span data-stu-id="bb78c-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="bb78c-111">I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.</span><span class="sxs-lookup"><span data-stu-id="bb78c-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="bb78c-112">Öppna meddelandet som du vill återkalla.</span><span class="sxs-lookup"><span data-stu-id="bb78c-112">Open the message that you want to recall.</span></span> <span data-ttu-id="bb78c-113">Du måste dubbelklicka för att öppna meddelandet.</span><span class="sxs-lookup"><span data-stu-id="bb78c-113">You must double-click to open the message.</span></span> <span data-ttu-id="bb78c-114">Om du väljer meddelandet så att det visas i Läs fönstret kan du inte återkalla meddelandet.</span><span class="sxs-lookup"><span data-stu-id="bb78c-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="bb78c-115">Välj **åtgärder**  >  **återkalla detta meddelande**på fliken meddelande.</span><span class="sxs-lookup"><span data-stu-id="bb78c-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="bb78c-116">Välj **ta bort olästa exemplar av detta meddelande** eller **ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="bb78c-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="bb78c-117">Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="bb78c-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="bb78c-118">Om du har problem med att återkalla meddelanden beror det på mottagarens inställningar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="bb78c-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="bb78c-119">Mer information om hur du kontrollerar åter kallelsen finns i [återkalla eller ersätta ett e-postmeddelande som du har skickat](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="bb78c-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="bb78c-120">***Söka efter och ta bort e-postmeddelanden i din organisation*** Om du är global administratör kan du söka efter och ta bort e-postmeddelanden i organisationen. Om du inte är global administratör måste ditt konto läggas till i roll gruppen för eDiscovery-hanteraren eller till en hanterings roll för Sök efter efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="bb78c-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="bb78c-121">Om du vill ta bort meddelanden måste du gå med i roll gruppen organisations hantering eller rollen för sökning och rensning.</span><span class="sxs-lookup"><span data-stu-id="bb78c-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="bb78c-122">Behörigheter för dessa roller är tilldelade i [säkerhets & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bb78c-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="bb78c-123">[Skapa en innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.</span><span class="sxs-lookup"><span data-stu-id="bb78c-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="bb78c-124">[Anslut till säkerhets & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="bb78c-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="bb78c-125">Om du använder MFA kan du läsa [Anslut till Microsoft 365 security & Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="bb78c-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
