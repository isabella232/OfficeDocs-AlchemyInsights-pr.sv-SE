---
title: Fil öppen skrivskyddad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702792"
---
# <a name="file-open-read-only"></a><span data-ttu-id="3fec6-102">Fil öppen skrivskyddad</span><span class="sxs-lookup"><span data-stu-id="3fec6-102">File open read-only</span></span>

<span data-ttu-id="3fec6-103">Du kanske upptäcker att när du öppnar filer öppnas de som skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="3fec6-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="3fec6-104">I vissa fall är detta för ökad säkerhet, till exempel när du öppnar filer från Internet, och andra gånger kan det bero på en inställning som kan ändras.</span><span class="sxs-lookup"><span data-stu-id="3fec6-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="3fec6-105">Här är några scenarier där en fil öppnas skrivskyddad och några åtgärder du kan vidta för att ändra det.</span><span class="sxs-lookup"><span data-stu-id="3fec6-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="3fec6-106">**Antivirusprogrammet gör att de öppnas skrivskyddat**</span><span class="sxs-lookup"><span data-stu-id="3fec6-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="3fec6-107">Vissa antivirusprogram kan skydda dig från potentiellt osäkra filer genom att öppna dem skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="3fec6-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="3fec6-108">Du kan behöva kontrollera med antivirusleverantören för att lära dig hur du justerar dessa inställningar.</span><span class="sxs-lookup"><span data-stu-id="3fec6-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="3fec6-109">BitDefender, till exempel, har innehåll på att lägga till programundanskap här: [Så här lägger du till program- eller processundanslutningar i Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="3fec6-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="3fec6-110">**Är filegenskaperna skrivskyddade?**</span><span class="sxs-lookup"><span data-stu-id="3fec6-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="3fec6-111">Du kan kontrollera filegenskaperna genom att högerklicka på filen och välja Egenskaper.</span><span class="sxs-lookup"><span data-stu-id="3fec6-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="3fec6-112">Om attributet Skrivskyddat är markerat kan du avmarkera det och klicka på OK.</span><span class="sxs-lookup"><span data-stu-id="3fec6-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="3fec6-113">**Innehållet är i skyddad vy**</span><span class="sxs-lookup"><span data-stu-id="3fec6-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="3fec6-114">Filer från Internet och från andra potentiellt osäkra platser kan innehålla virus, maskar eller andra typer av skadlig kod som kan skada datorn.</span><span class="sxs-lookup"><span data-stu-id="3fec6-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="3fec6-115">Detta är också vanligt med e-postbilagor eller filer som du har laddat ned.</span><span class="sxs-lookup"><span data-stu-id="3fec6-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="3fec6-116">För att skydda datorn öppnas filer från dessa potentiellt osäkra platser i skyddad vy.</span><span class="sxs-lookup"><span data-stu-id="3fec6-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="3fec6-117">Genom att använda skyddad vy kan du läsa en fil och se dess innehåll samtidigt som du minskar riskerna.</span><span class="sxs-lookup"><span data-stu-id="3fec6-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="3fec6-118">Mer information om skyddad vy och hur du ändrar inställningar finns i den här artikeln: [Vad är skyddad vy?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="3fec6-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="3fec6-119">**Är OneDrive fullt?**</span><span class="sxs-lookup"><span data-stu-id="3fec6-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="3fec6-120">Om filen lagras på OneDrive och lagringsutrymmet för OneDrive är fullt kan du inte spara dokumentet förrän du befinner dig under det tilldelade utrymmet.</span><span class="sxs-lookup"><span data-stu-id="3fec6-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="3fec6-121">Du kan kontrollera ditt lediga utrymme på OneDrive genom att klicka på OneDrive-ikonen [https://onedrive.live.com](https://onedrive.live.com)i meddelandecentret och välja Hantera lagringsutrymme, eller så kan du gå till , logga in och notera mängden använt utrymme längst ned till vänster på skärmen.</span><span class="sxs-lookup"><span data-stu-id="3fec6-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="3fec6-122">**Är Office aktiverat?**</span><span class="sxs-lookup"><span data-stu-id="3fec6-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="3fec6-123">Om Office inte är aktiverat, eller om din prenumeration har upphört att gälla, kan du vara i skrivskyddat läge nedsatt funktionalitet.</span><span class="sxs-lookup"><span data-stu-id="3fec6-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="3fec6-124">Information om hur du aktiverar Office finns [i: Olicensierad produkt och aktiveringsfel i Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3fec6-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="3fec6-125">**Om allt annat misslyckas...**</span><span class="sxs-lookup"><span data-stu-id="3fec6-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="3fec6-126">Prova att starta om datorn</span><span class="sxs-lookup"><span data-stu-id="3fec6-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="3fec6-127">Installera Office-uppdateringar</span><span class="sxs-lookup"><span data-stu-id="3fec6-127">Install Office updates</span></span>
    
- <span data-ttu-id="3fec6-128">Utföra en onlinereparation av Office</span><span class="sxs-lookup"><span data-stu-id="3fec6-128">Perform an Online repair of Office</span></span>
    

