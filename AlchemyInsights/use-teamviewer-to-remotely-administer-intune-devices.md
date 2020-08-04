---
title: Använda TeamViewer för att fjärrdministrera Intune-enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555751"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="2a43a-102">Använda TeamViewer för att fjärrdministrera Intune-enheter</span><span class="sxs-lookup"><span data-stu-id="2a43a-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="2a43a-103">Enheter som hanteras av Intune kan fjärrges med [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="2a43a-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="2a43a-104">Så här administrerar du Intune med TeamViewer:</span><span class="sxs-lookup"><span data-stu-id="2a43a-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="2a43a-105">Börja med att hämta autentiseringsuppgifter från TeamViewer för att konfigurera TeamViewer Connector på Intune.</span><span class="sxs-lookup"><span data-stu-id="2a43a-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="2a43a-106">På så sätt kan administratören ange autentiseringsuppgifter i TeamViewer Connector-användargränssnittet under Enheter, en engångsåtgärd för att upprätta länken mellan Intune och TeamViewer-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="2a43a-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="2a43a-107">**Del 1: Starta en session med en fjärrenhet**</span><span class="sxs-lookup"><span data-stu-id="2a43a-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="2a43a-108">Under **Alla enheter**väljer du den enhet som du vill starta en fjärrsession med.</span><span class="sxs-lookup"><span data-stu-id="2a43a-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="2a43a-109">Från **... Mer**väljer du **Ny fjärrhjälpssession**.</span><span class="sxs-lookup"><span data-stu-id="2a43a-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="2a43a-110">Välj **Ja** för att bekräfta att du vill upprätta en fjärrsession.</span><span class="sxs-lookup"><span data-stu-id="2a43a-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="2a43a-111">När begäran om att initiera en ny fjärrsession har bekräftats av TeamViewer-tjänsten visas ett alternativ för att **starta fjärrhjälp** under information om fönstret Översikt (eller Essentials) för enheten.</span><span class="sxs-lookup"><span data-stu-id="2a43a-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="2a43a-112">Välj **Visa mer** om du vill expandera fönstret och visa fjärrhjälpsstatus.</span><span class="sxs-lookup"><span data-stu-id="2a43a-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="2a43a-113">Välj **Starta fjärrsession** om du vill starta sessionen på administratörssidan.</span><span class="sxs-lookup"><span data-stu-id="2a43a-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="2a43a-114">Välj att hämta Den binära TeamViewer (Windows) och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="2a43a-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="2a43a-115">**Anm.)** Du kan ignorera alla webbläsar sidor öppnas till TeamViewer webbplats.</span><span class="sxs-lookup"><span data-stu-id="2a43a-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="2a43a-116">Bekräfta begäran om att TeamViewer-appen ska göra ändringar på enheten (endast Windows).</span><span class="sxs-lookup"><span data-stu-id="2a43a-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="2a43a-117">TeamViewer-appen startar och innehåller sessionskoden för att autentisera anslutningen med fjärrenheten.</span><span class="sxs-lookup"><span data-stu-id="2a43a-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="2a43a-118">**Del 2: På den enhet som är avsedd för en fjärrsession**</span><span class="sxs-lookup"><span data-stu-id="2a43a-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="2a43a-119">Öppna Företagsportalen Intune.</span><span class="sxs-lookup"><span data-stu-id="2a43a-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="2a43a-120">Leta efter en aviseringsflagga: "IT-administratören begär kontroll över den här enheten för en fjärrhjälpssession" och väljer meddelandet.</span><span class="sxs-lookup"><span data-stu-id="2a43a-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="2a43a-121">Välj att ladda ned TeamViewer-programmet eller bekräfta nedladdningen av TeamViewer-appen från App Store och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="2a43a-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="2a43a-122">**Anm.)** Du kan ignorera alla webbläsar sidor öppnas till TeamViewer webbplats.</span><span class="sxs-lookup"><span data-stu-id="2a43a-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="2a43a-123">Bekräfta begäran om att TeamViewer-appen ska göra ändringar på enheten (endast Windows).</span><span class="sxs-lookup"><span data-stu-id="2a43a-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="2a43a-124">TeamViewer-appen startar och innehåller sessionskoden för att autentisera anslutningen med fjärrenheten.</span><span class="sxs-lookup"><span data-stu-id="2a43a-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="2a43a-125">En popup frågar om du vill tillåta sessionen att starta.</span><span class="sxs-lookup"><span data-stu-id="2a43a-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="2a43a-126">**Anm.)** De sessionskoder som genereras av TeamViewer-tjänsten används endast en gång.</span><span class="sxs-lookup"><span data-stu-id="2a43a-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="2a43a-127">Om du förlorar anslutningen måste du:</span><span class="sxs-lookup"><span data-stu-id="2a43a-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="2a43a-128">Stäng instansen av TeamViewer-appen på fjärrenheten och på administratörsarbetsstationen.</span><span class="sxs-lookup"><span data-stu-id="2a43a-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="2a43a-129">Stäng företagsportalen på fjärrenheten.</span><span class="sxs-lookup"><span data-stu-id="2a43a-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="2a43a-130">Starta en ny "Ny fjärrhjälpssession" från administratörsportalen.</span><span class="sxs-lookup"><span data-stu-id="2a43a-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="2a43a-131">Öppna företagsportalen på fjärrenheten igen för att ta emot det nya meddelandet.</span><span class="sxs-lookup"><span data-stu-id="2a43a-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="2a43a-132">Ladda ned och öppna TeamViewer-appen på både fjärrenheten och administratörsarbetsstationen, som tidigare.</span><span class="sxs-lookup"><span data-stu-id="2a43a-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>