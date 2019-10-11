---
title: Fastnat i Utkorgen på grund av stora bilagor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441323"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="552f7-102">Åtgärda meddelanden som har fastnat i Utkorgen</span><span class="sxs-lookup"><span data-stu-id="552f7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="552f7-103">Vi rekommenderar att du börjar med att köra scenariot ["Jag har problem med att skicka, ta emot eller hitta e-postmeddelanden"](https://aka.ms/SaRA-OutlookSendReceive) från verktyget [Microsoft support och återställning assistenten](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="552f7-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="552f7-104">När ett meddelande fastnar i Utkorgen är de mest troliga orsakerna:</span><span class="sxs-lookup"><span data-stu-id="552f7-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="552f7-105">Stora bilagor.</span><span class="sxs-lookup"><span data-stu-id="552f7-105">Large attachments.</span></span>
- <span data-ttu-id="552f7-106">Alternativet **Skicka omedelbart när anslutet** är inte aktiverat.</span><span class="sxs-lookup"><span data-stu-id="552f7-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="552f7-107">Så här tar du bort stora bilagor:</span><span class="sxs-lookup"><span data-stu-id="552f7-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="552f7-108">I Outlook väljer du **skicka och ta emot** > **arbete offline**.</span><span class="sxs-lookup"><span data-stu-id="552f7-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="552f7-109">Välj **Utkorg**i navigeringsfönstret.</span><span class="sxs-lookup"><span data-stu-id="552f7-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="552f7-110">Härifrån kan du:</span><span class="sxs-lookup"><span data-stu-id="552f7-110">From here, you can:</span></span> 
    - <span data-ttu-id="552f7-111">Ta bort meddelandet (Markera det och välj sedan **ta bort**).</span><span class="sxs-lookup"><span data-stu-id="552f7-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="552f7-112">Dra meddelandet till mappen Utkast, dubbelklicka för att öppna det och ta bort bilagan Markera den och välj sedan **ta bort**).</span><span class="sxs-lookup"><span data-stu-id="552f7-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="552f7-113">Om du får ett felmeddelande som säger att Outlook försöker skicka meddelandet stänger du Outlook.</span><span class="sxs-lookup"><span data-stu-id="552f7-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="552f7-114">Det kan ta en stund att avsluta.</span><span class="sxs-lookup"><span data-stu-id="552f7-114">It may take a few moments to exit.</span></span> <span data-ttu-id="552f7-115">Om Outlook inte stängs trycker du på Ctrl + Alt + Delete och väljer **Starta Aktivitetshanteraren**.</span><span class="sxs-lookup"><span data-stu-id="552f7-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="552f7-116">I Aktivitetshanteraren väljer du fliken **processer** , bläddrar ned till Outlook. exe och väljer **Avsluta process**.</span><span class="sxs-lookup"><span data-stu-id="552f7-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="552f7-117">När Outlook har stängts startar du om det och upprepar steg 2 och 3.</span><span class="sxs-lookup"><span data-stu-id="552f7-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="552f7-118">När du tar bort den bifogade filen klickar du på **skicka och ta emot** > **arbete offline** att återuppta arbeta online.</span><span class="sxs-lookup"><span data-stu-id="552f7-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="552f7-119">Meddelanden fastnar också i Utkorgen när du klickar på **Skicka**, men du är inte ansluten.</span><span class="sxs-lookup"><span data-stu-id="552f7-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="552f7-120">Klicka på **skicka och ta emot** och titta på knappen **arbeta offline** .</span><span class="sxs-lookup"><span data-stu-id="552f7-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="552f7-121">Om det är blått är du frånkopplad.</span><span class="sxs-lookup"><span data-stu-id="552f7-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="552f7-122">Välj den för att ansluta (knappen blir vit) och klicka på **skicka alla**.</span><span class="sxs-lookup"><span data-stu-id="552f7-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="552f7-123">Så här aktiverar du **Skicka omedelbart vid anslutning**:</span><span class="sxs-lookup"><span data-stu-id="552f7-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="552f7-124">Välj **fil** > **alternativ** >  **Avancerat**.</span><span class="sxs-lookup"><span data-stu-id="552f7-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="552f7-125">I avsnittet **skicka och ta emot** väljer du **Skicka omedelbart när du är ansluten**och väljer sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="552f7-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="552f7-126">För fullständig information se:</span><span class="sxs-lookup"><span data-stu-id="552f7-126">For full details see:</span></span>
- [<span data-ttu-id="552f7-127">Video: skicka eller ta bort en fast e-post</span><span class="sxs-lookup"><span data-stu-id="552f7-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="552f7-128">E-post stannar i mappen Utkorg tills du manuellt initiera en skicka/ta emot-åtgärd i Outlook</span><span class="sxs-lookup"><span data-stu-id="552f7-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
