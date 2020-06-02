---
title: Återkalla eller ersätta ett e-postmeddelande i Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502337"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="b4eb0-102">Återkalla eller ersätta ett Outlook-e-postmeddelande</span><span class="sxs-lookup"><span data-stu-id="b4eb0-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="b4eb0-103">Som administratör kan du **återkalla meddelanden för användare som använder PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b4eb0-104">Du kan inte återkalla meddelanden från administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b4eb0-105">Du kan **bara återkalla meddelanden som skickas till personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b4eb0-106">Om meddelandet till exempel skickades till en Gmail-adress kan du inte komma ihåg det.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b4eb0-107">Du kan **bara återkalla meddelanden som skickas från Outlook 2016 på datorn**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b4eb0-108">Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b4eb0-109">Så här återkallar eller ersätter du ett e-postmeddelande:</span><span class="sxs-lookup"><span data-stu-id="b4eb0-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b4eb0-110">Välj mappen Skickat i mappfönstret till vänster om Outlook-fönstret.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b4eb0-111">Dubbelklicka på meddelandet som du vill återkalla för att öppna det.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b4eb0-112">Markera fliken **Meddelande** och välj sedan **Åtgärder**  >  **återkalla det här meddelandet**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b4eb0-113">Välj **Ta bort olästa kopior av meddelandet** eller Ta bort **olästa kopior och ersätt med ett nytt meddelande**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b4eb0-114">Om du skickar ett ersättningsmeddelande skriver du meddelandet och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b4eb0-115">Hur ett meddelande återkallas eller misslyckas beror på mottagarens inställningar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b4eb0-116">Steg för att kontrollera återkallandet finns i den [här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b4eb0-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b4eb0-117">Söka efter och ta bort e-postmeddelanden i organisationen</span><span class="sxs-lookup"><span data-stu-id="b4eb0-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b4eb0-118">Om du inte är global administratör måste ditt konto läggas till i rollen eDiscovery Manager eller hanteringsrollen för efterlevnadssökning för att söka efter meddelanden.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b4eb0-119">Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller hanteringsrollen Sök och rensa.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b4eb0-120">Behörigheter för dessa roller tilldelas i [säkerhets- och efterlevnadscentret](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="b4eb0-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b4eb0-121">[Skapa en innehållssökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b4eb0-122">[Anslut till Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b4eb0-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b4eb0-123">Om du använder multifaktorautentisering läser du [Anslut till Microsoft 365 security and Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b4eb0-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>