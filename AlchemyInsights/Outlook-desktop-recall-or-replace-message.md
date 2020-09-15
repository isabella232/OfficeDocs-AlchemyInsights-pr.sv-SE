---
title: Skriv bords versionen av Outlook eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664008"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7c6a0-102">Återkalla eller ersätta ett e-postmeddelande i Outlook</span><span class="sxs-lookup"><span data-stu-id="7c6a0-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7c6a0-103">Som administratör kan du **återkalla meddelanden åt användare med hjälp av PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7c6a0-104">Du kan inte återkalla meddelanden från administrations centret.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7c6a0-105">Du kan **bara återkalla meddelanden som skickas till personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7c6a0-106">Om meddelandet skickades till en Gmail-adress, till exempel, kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7c6a0-107">Du kan **bara återkalla meddelanden som skickats från Outlook 2016 på datorn**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7c6a0-108">Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben kan du inte återkalla det.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7c6a0-109">Så här återkallar eller ersätter du ett e-postmeddelande:</span><span class="sxs-lookup"><span data-stu-id="7c6a0-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7c6a0-110">I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7c6a0-111">Dubbelklicka på det meddelande som du vill återkalla för att öppna det.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7c6a0-112">Välj fliken **meddelande** och sedan **åtgärder**  >  **återkalla detta meddelande**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7c6a0-113">Välj **ta bort olästa exemplar av detta meddelande** eller **ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7c6a0-114">Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7c6a0-115">Om du har problem med att återkalla meddelanden beror det på mottagarens inställningar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7c6a0-116">Anvisningar för hur du kontrollerar åter kallelsen finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7c6a0-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7c6a0-117">Söka efter och ta bort e-postmeddelanden i din organisation</span><span class="sxs-lookup"><span data-stu-id="7c6a0-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7c6a0-118">Om du inte är global administratör måste ditt konto läggas till i eDiscovery Manager-rollen eller för Sök hanterings rollen efterlevnad för att söka efter meddelanden.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7c6a0-119">Om du vill ta bort meddelanden måste du gå med i roll gruppen organisations hantering eller rollen för sökning och rensning.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7c6a0-120">Behörigheter för dessa roller är tilldelade i [säkerhets-och kompatibilitetstillstånd](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7c6a0-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7c6a0-121">[Skapa en innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.</span><span class="sxs-lookup"><span data-stu-id="7c6a0-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7c6a0-122">[Anslut till säkerhets-och Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7c6a0-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7c6a0-123">Om du använder multifaktorautentisering läser du [ansluta till Microsoft 365 Security och Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7c6a0-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>