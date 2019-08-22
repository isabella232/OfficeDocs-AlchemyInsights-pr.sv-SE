---
title: Outlook stationära återkalla eller ersätta ett e-postmeddelande
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496129"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="77030-102">Återkalla eller ersätta ett e-postmeddelande i Outlook</span><span class="sxs-lookup"><span data-stu-id="77030-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="77030-103">Som administratör kan du **Återkalla meddelanden för användare med hjälp av PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="77030-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="77030-104">Du kan inte återkalla meddelanden från administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="77030-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="77030-105">Du kan **bara återkalla meddelanden som skickas till personer i din organisation**.</span><span class="sxs-lookup"><span data-stu-id="77030-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="77030-106">Om meddelandet har skickats till en Gmail-adress, till exempel du inte kommer ihåg den.</span><span class="sxs-lookup"><span data-stu-id="77030-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="77030-107">Du kan **bara återkalla meddelanden som skickas från Outlook 2016 på datorn**.</span><span class="sxs-lookup"><span data-stu-id="77030-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="77030-108">Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben, du kan inte återkalla den.</span><span class="sxs-lookup"><span data-stu-id="77030-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="77030-109">Att återkalla eller ersätta ett e-postmeddelande:</span><span class="sxs-lookup"><span data-stu-id="77030-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="77030-110">Markera mappen Skickat i mappfönstret till vänster i Outlook-fönstret.</span><span class="sxs-lookup"><span data-stu-id="77030-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="77030-111">Dubbelklicka på meddelandet som du vill återkalla om du vill öppna den.</span><span class="sxs-lookup"><span data-stu-id="77030-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="77030-112">Klicka på fliken **meddelande** och välj **åtgärder** > **Återkalla detta meddelande**.</span><span class="sxs-lookup"><span data-stu-id="77030-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="77030-113">Välj **Ta bort olästa exemplar av meddelandet** eller **Ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="77030-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="77030-114">Om du skickar ett meddelande med ersättning, skriver meddelandet och välj sedan **Skicka**.</span><span class="sxs-lookup"><span data-stu-id="77030-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="77030-115">Lyckades eller inte återkalla ett meddelande beror på mottagarens inställningar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="77030-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="77030-116">Åtgärder för att kontrollera om återkallelsen, finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="77030-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="77030-117">Söka efter och ta bort e-postmeddelanden i organisationen</span><span class="sxs-lookup"><span data-stu-id="77030-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="77030-118">Om du inte är en global administratör måste ditt konto läggas till e-informationsavslöjande Manager roll eller överensstämmelse Search management rollen att söka efter meddelanden.</span><span class="sxs-lookup"><span data-stu-id="77030-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="77030-119">Om du vill ta bort meddelanden, måste du ansluta till organisationshantering roll gruppen eller rollen för sökning och rensa.</span><span class="sxs-lookup"><span data-stu-id="77030-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="77030-120">Behörigheter för rollerna tilldelas i [center för säkerhet och kompatibilitet](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="77030-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="77030-121">[Skapa ett innehåll söka](https://docs.microsoft.com/office365/securitycompliance/content-search) efter meddelandet om du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="77030-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="77030-122">[Ansluta till säkerhet och PowerShell regelefterlevnadscentret](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="77030-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="77030-123">Om du använder autentisering på flera plan finns i [Anslut till Office 365 säkerhet och regelefterlevnad Center PowerShell använda autentisering på flera plan](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="77030-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>