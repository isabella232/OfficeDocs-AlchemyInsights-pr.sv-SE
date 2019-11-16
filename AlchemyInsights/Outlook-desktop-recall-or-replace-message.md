---
title: Outlook-skrivbordet återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496129"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="5666d-102">Återkalla eller ersätta ett Outlook-e-postmeddelande</span><span class="sxs-lookup"><span data-stu-id="5666d-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="5666d-103">Som administratör kan du **återkalla meddelanden för användare med hjälp av PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="5666d-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="5666d-104">Du kan inte återkalla meddelanden från administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="5666d-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="5666d-105">Du kan **bara återkalla meddelanden som skickas till personer i din organisation**.</span><span class="sxs-lookup"><span data-stu-id="5666d-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="5666d-106">Om meddelandet skickades till en Gmail-adress kan du till exempel inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="5666d-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="5666d-107">Du kan **bara återkalla meddelanden som skickats från Outlook 2016 på datorn**.</span><span class="sxs-lookup"><span data-stu-id="5666d-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="5666d-108">Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="5666d-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="5666d-109">Så här återkallar eller ersätter du ett e-postmeddelande:</span><span class="sxs-lookup"><span data-stu-id="5666d-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="5666d-110">I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.</span><span class="sxs-lookup"><span data-stu-id="5666d-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="5666d-111">Dubbelklicka på det meddelande som du vill återkalla för att öppna det.</span><span class="sxs-lookup"><span data-stu-id="5666d-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="5666d-112">Välj fliken **meddelande** och välj sedan **åtgärder** > **återkalla det här meddelandet**.</span><span class="sxs-lookup"><span data-stu-id="5666d-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="5666d-113">Välj **ta bort olästa kopior av det här meddelandet** eller **ta bort olästa kopior och Ersätt med ett nytt meddelande**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="5666d-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="5666d-114">Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="5666d-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="5666d-115">Lyckade eller misslyckade återkallningar av ett meddelande beror på mottagarens inställningar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="5666d-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="5666d-116">Anvisningar om hur du kontrollerar återkallningen finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="5666d-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="5666d-117">Sök efter och ta bort e-postmeddelanden i din organisation</span><span class="sxs-lookup"><span data-stu-id="5666d-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="5666d-118">Om du inte är global administratör måste ditt konto läggas till i rollen eDiscovery Manager-roll eller efterlevnadshantering för att söka efter meddelanden.</span><span class="sxs-lookup"><span data-stu-id="5666d-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="5666d-119">Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller rollen Sök-och rensnings hantering.</span><span class="sxs-lookup"><span data-stu-id="5666d-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="5666d-120">Behörigheter för dessa roller tilldelas i säkerhets- [och Efterlevnadscenter](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="5666d-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="5666d-121">[Skapa en innehållssökning](https://docs.microsoft.com/office365/securitycompliance/content-search) för att hitta meddelandet att ta bort.</span><span class="sxs-lookup"><span data-stu-id="5666d-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="5666d-122">[Anslut till Security och Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="5666d-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="5666d-123">Om du använder multifaktorautentisering, se [ansluta till Office 365 Security och Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="5666d-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>