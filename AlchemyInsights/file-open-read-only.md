---
title: Öppna med skrivskydd
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813202"
---
# <a name="file-open-read-only"></a><span data-ttu-id="07b14-102">Öppna med skrivskydd</span><span class="sxs-lookup"><span data-stu-id="07b14-102">File open read-only</span></span>

<span data-ttu-id="07b14-103">Det kan hända att filer öppnas med skrivskydd när du öppnar dem.</span><span class="sxs-lookup"><span data-stu-id="07b14-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="07b14-104">I vissa fall kan det här vara ett skydd för ökad säkerhet, till exempel när du öppnar filer från Internet och andra gånger kan det bero på en inställning som kan ändras.</span><span class="sxs-lookup"><span data-stu-id="07b14-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="07b14-105">Här är några scenarier där en fil öppnas med skrivskydd och några åtgärder du kan vidta för att ändra det.</span><span class="sxs-lookup"><span data-stu-id="07b14-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="07b14-106">**Mitt antivirusprogram gör så att de öppnas med skrivskydd**</span><span class="sxs-lookup"><span data-stu-id="07b14-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="07b14-107">Vissa antivirusprogram kan skydda dig från potentiellt osäkra filer genom att öppna dem skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="07b14-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="07b14-108">Du kan behöva kontrollera med din antivirusleverantör för att lära dig hur du justerar dessa inställningar.</span><span class="sxs-lookup"><span data-stu-id="07b14-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="07b14-109">BitDefender har till exempel innehåll om att lägga till undantag för program här: Så här lägger du till undantag för program eller processer i [Bitdefender Control Center.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="07b14-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="07b14-110">**Är filegenskaperna inställda på skrivskydd?**</span><span class="sxs-lookup"><span data-stu-id="07b14-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="07b14-111">Du kan kontrollera filegenskaperna genom att högerklicka på filen och välja Egenskaper.</span><span class="sxs-lookup"><span data-stu-id="07b14-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="07b14-112">Om attributet Skrivskyddad är markerat avmarkerar du det och klickar på OK.</span><span class="sxs-lookup"><span data-stu-id="07b14-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="07b14-113">**Innehållet är i skyddad vy**</span><span class="sxs-lookup"><span data-stu-id="07b14-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="07b14-114">Filer från Internet och andra eventuellt osäkra platser kan innehålla virus, maskar eller annan skadlig programvara som kan skada datorn.</span><span class="sxs-lookup"><span data-stu-id="07b14-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="07b14-115">Detta gäller även ofta e-postbilagor och nedladdade filer.</span><span class="sxs-lookup"><span data-stu-id="07b14-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="07b14-116">För att skydda datorn öppnas filer från sådana potentiellt osäkra platser i Skyddad vy.</span><span class="sxs-lookup"><span data-stu-id="07b14-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="07b14-117">Genom att använda Skyddad vy kan du läsa en fil och visa dess innehåll samtidigt som du minskar risken.</span><span class="sxs-lookup"><span data-stu-id="07b14-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="07b14-118">Mer information om Skyddad vy och hur du ändrar inställningar finns i den här artikeln: [Vad är Skyddad vy?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="07b14-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="07b14-119">**Är OneDrive fullt?**</span><span class="sxs-lookup"><span data-stu-id="07b14-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="07b14-120">Om filen lagras på OneDrive och ditt OneDrive-lagringsutrymme är fullt kan du inte spara dokumentet förrän det finns plats i ditt tilldelade utrymme.</span><span class="sxs-lookup"><span data-stu-id="07b14-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="07b14-121">Du kan kontrollera ditt lediga utrymme på OneDrive genom att klicka på OneDrive-ikonen i meddelandecentret och välja Hantera lagring. Du kan också gå till , logga in och anteckna mängden använt utrymme längst ned till vänster på [https://onedrive.live.com](https://onedrive.live.com) skärmen.</span><span class="sxs-lookup"><span data-stu-id="07b14-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="07b14-122">**Är Office aktiverat?**</span><span class="sxs-lookup"><span data-stu-id="07b14-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="07b14-123">Om Office inte är aktiverat, eller om prenumerationen har gått ut, kan du vara i det skrivskyddade läget Nedsatt funktionalitet.</span><span class="sxs-lookup"><span data-stu-id="07b14-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="07b14-124">Information om hur du aktiverar Office finns i: [Office-felmeddelanden om olicensierad produkt och aktivering.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="07b14-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="07b14-125">**Om allt annat misslyckas ...**</span><span class="sxs-lookup"><span data-stu-id="07b14-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="07b14-126">Försök starta om datorn</span><span class="sxs-lookup"><span data-stu-id="07b14-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="07b14-127">Installera Office-uppdateringar</span><span class="sxs-lookup"><span data-stu-id="07b14-127">Install Office updates</span></span>
    
- <span data-ttu-id="07b14-128">Utföra en onlinereparation av Office</span><span class="sxs-lookup"><span data-stu-id="07b14-128">Perform an Online repair of Office</span></span>
    

