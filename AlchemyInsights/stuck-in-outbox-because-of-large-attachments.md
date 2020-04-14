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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241270"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="c3094-102">Åtgärda meddelanden som har fastnat i utkorgen</span><span class="sxs-lookup"><span data-stu-id="c3094-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="c3094-103">Vi rekommenderar att du börjar med att köra scenariot ["Jag har problem med att skicka, ta emot eller hitta e-postmeddelanden"](https://aka.ms/SaRA-OutlookSendReceive) från verktyget [Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="c3094-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="c3094-104">När ett meddelande fastnar i utkorgen är den troligaste orsaken en stor bilaga eller alternativet "Skicka omedelbart när du är ansluten" är inte aktiverat.</span><span class="sxs-lookup"><span data-stu-id="c3094-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="c3094-105">**Ta bort den stora bilagan**</span><span class="sxs-lookup"><span data-stu-id="c3094-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="c3094-106">Välj **Skicka/ta emot** > **arbete offline**i Outlook .</span><span class="sxs-lookup"><span data-stu-id="c3094-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="c3094-107">Välj Utkorg i **navigeringsfönstret**.</span><span class="sxs-lookup"><span data-stu-id="c3094-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="c3094-108">Härifrån kan du:</span><span class="sxs-lookup"><span data-stu-id="c3094-108">From here, you can:</span></span> 
    - <span data-ttu-id="c3094-109">Ta bort meddelandet (markera det och välj sedan **Ta bort**).</span><span class="sxs-lookup"><span data-stu-id="c3094-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="c3094-110">Dra meddelandet till mappen Utkast, dubbelklicka för att öppna det och ta bort den bifogade filen och markera det sedan och välj sedan **Ta bort**).</span><span class="sxs-lookup"><span data-stu-id="c3094-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="c3094-111">Om du får ett felmeddelande om att Outlook försöker överföra meddelandet stänger du Outlook.</span><span class="sxs-lookup"><span data-stu-id="c3094-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="c3094-112">Det kan ta en stund att avsluta.</span><span class="sxs-lookup"><span data-stu-id="c3094-112">It may take a few moments to exit.</span></span> <span data-ttu-id="c3094-113">Om Outlook inte stängs trycker du på Ctrl+Alt+Delete och väljer **Starta Aktivitetshanteraren**.</span><span class="sxs-lookup"><span data-stu-id="c3094-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="c3094-114">I **Aktivitetshanteraren** väljer du fliken Processer, rullar ned till outlook.exe och väljer **Avsluta process**.</span><span class="sxs-lookup"><span data-stu-id="c3094-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="c3094-115">När Outlook har stängts startar du om det och upprepar steg 2 och 3.</span><span class="sxs-lookup"><span data-stu-id="c3094-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="c3094-116">När du har tagit bort den bifogade filen klickar du på **Skicka/ta emot** > **arbete offline** för att fortsätta arbeta online.</span><span class="sxs-lookup"><span data-stu-id="c3094-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="c3094-117">Meddelanden fastnar också i utkorgen när du klickar på **Skicka**, men du är inte ansluten.</span><span class="sxs-lookup"><span data-stu-id="c3094-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="c3094-118">Klicka på **Skicka/ta emot** och titta på knappen **Arbeta offline.**</span><span class="sxs-lookup"><span data-stu-id="c3094-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="c3094-119">Om den är blå är du frånkopplad.</span><span class="sxs-lookup"><span data-stu-id="c3094-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="c3094-120">Klicka på den för att ansluta (knappen blir vit) och klicka på **Skicka alla**.</span><span class="sxs-lookup"><span data-stu-id="c3094-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="c3094-121">**Aktivera Skicka direkt när du är ansluten**</span><span class="sxs-lookup"><span data-stu-id="c3094-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="c3094-122">Klicka på **Alternativ**på fliken Arkiv .</span><span class="sxs-lookup"><span data-stu-id="c3094-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="c3094-123">Klicka på **Avancerat**i dialogrutan Outlook-alternativ .</span><span class="sxs-lookup"><span data-stu-id="c3094-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="c3094-124">I avsnittet Skicka och ta emot klickar du för att aktivera **Skicka direkt när du är ansluten**.</span><span class="sxs-lookup"><span data-stu-id="c3094-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="c3094-125">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="c3094-125">Click **OK**.</span></span>
 
<span data-ttu-id="c3094-126">För fullständig information, se:</span><span class="sxs-lookup"><span data-stu-id="c3094-126">For full details, see:</span></span>
- [<span data-ttu-id="c3094-127">Video: Skicka eller ta bort ett fast e-postmeddelande</span><span class="sxs-lookup"><span data-stu-id="c3094-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="c3094-128">E-post finns kvar i mappen Utkorgen tills du initierar en skicka/ta-mottagning i Outlook manuellt</span><span class="sxs-lookup"><span data-stu-id="c3094-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
