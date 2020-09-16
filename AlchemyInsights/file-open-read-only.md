---
title: Filen är skrivskyddad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745625"
---
# <a name="file-open-read-only"></a><span data-ttu-id="c7404-102">Filen är skrivskyddad</span><span class="sxs-lookup"><span data-stu-id="c7404-102">File open read-only</span></span>

<span data-ttu-id="c7404-103">Om du öppnar filer kanske de är skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="c7404-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="c7404-104">I vissa fall är detta för ökad säkerhet, till exempel när du öppnar filer från Internet, och andra gånger kan det bero på en inställning som kan ändras.</span><span class="sxs-lookup"><span data-stu-id="c7404-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="c7404-105">Här är några scenarier där en fil öppnas som skrivskyddad och några steg som du kan vidta för att ändra.</span><span class="sxs-lookup"><span data-stu-id="c7404-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="c7404-106">**Mitt antivirus program gör att de öppnas med skriv skydd**</span><span class="sxs-lookup"><span data-stu-id="c7404-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="c7404-107">Vissa antivirus program skyddar dig från potentiellt osäkra filer genom att öppna dem som skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="c7404-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="c7404-108">Du kan behöva kolla med din antivirus leverantör för att lära dig hur du justerar dessa inställningar.</span><span class="sxs-lookup"><span data-stu-id="c7404-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="c7404-109">BitDefender har till exempel innehåll om att lägga till program undantag här: [så här lägger du till program eller process undantag i BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="c7404-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="c7404-110">**Är fil egenskaperna skrivskyddade?**</span><span class="sxs-lookup"><span data-stu-id="c7404-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="c7404-111">Du kan kontrol lera fil egenskaperna genom att högerklicka på filen och välja egenskaper.</span><span class="sxs-lookup"><span data-stu-id="c7404-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="c7404-112">Om det skrivskyddade attributet är markerat kan du avmarkera det och klicka på OK.</span><span class="sxs-lookup"><span data-stu-id="c7404-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="c7404-113">**Innehållet är i skyddad vy**</span><span class="sxs-lookup"><span data-stu-id="c7404-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="c7404-114">Filer från Internet och andra potentiellt osäkra platser kan innehålla virus, maskar eller andra typer av skadlig kod som kan skada din dator.</span><span class="sxs-lookup"><span data-stu-id="c7404-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="c7404-115">Det är vanligt vis fallet med e-postbilagor eller filer som du har laddat ner.</span><span class="sxs-lookup"><span data-stu-id="c7404-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="c7404-116">För att skydda din dator öppnas filer från de här osäkra platserna i skyddad vy.</span><span class="sxs-lookup"><span data-stu-id="c7404-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="c7404-117">Genom att använda skyddad vy kan du läsa en fil och se innehållet i den samtidigt som du minskar riskerna.</span><span class="sxs-lookup"><span data-stu-id="c7404-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="c7404-118">Mer information om skyddad vy och hur du ändrar inställningar finns i den här artikeln: [Vad är skyddad vy?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="c7404-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="c7404-119">**Är OneDrive fullt?**</span><span class="sxs-lookup"><span data-stu-id="c7404-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="c7404-120">Om filen är lagrad på OneDrive och OneDrive-utrymmet är fullt kan du inte spara dokumentet förrän du befinner dig under det tilldelade utrymmet.</span><span class="sxs-lookup"><span data-stu-id="c7404-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="c7404-121">Du kan kontrol lera hur mycket ledigt utrymme du har på OneDrive genom att klicka på OneDrive-ikonen i meddelande Center och välja Hantera lagring, eller så kan du gå till [https://onedrive.live.com](https://onedrive.live.com) , logga in och notera utrymmet längst ned till vänster på skärmen.</span><span class="sxs-lookup"><span data-stu-id="c7404-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="c7404-122">**Är Office aktiverat?**</span><span class="sxs-lookup"><span data-stu-id="c7404-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="c7404-123">Om Office inte är aktiverat eller om prenumerationen har gått ut kan du vara i läget skrivskyddad funktionalitet.</span><span class="sxs-lookup"><span data-stu-id="c7404-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="c7404-124">Information om hur du aktiverar Office finns i: [olicensierad produkt och aktiverings fel i Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="c7404-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="c7404-125">**Om det inte fungerar alls...**</span><span class="sxs-lookup"><span data-stu-id="c7404-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="c7404-126">Prova att starta om datorn</span><span class="sxs-lookup"><span data-stu-id="c7404-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="c7404-127">Installera Office-uppdateringar</span><span class="sxs-lookup"><span data-stu-id="c7404-127">Install Office updates</span></span>
    
- <span data-ttu-id="c7404-128">Utföra en online-reparation av Office</span><span class="sxs-lookup"><span data-stu-id="c7404-128">Perform an Online repair of Office</span></span>
    

