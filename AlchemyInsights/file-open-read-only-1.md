---
title: Filen öppnas i skrivskyddat läge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 117b1e24d6250a1d5eb092a01a0d5146d09ea2e5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401655"
---
# <a name="file-open-read-only"></a><span data-ttu-id="d8b7a-102">Filen öppnas i skrivskyddat läge</span><span class="sxs-lookup"><span data-stu-id="d8b7a-102">File open read-only</span></span>

<span data-ttu-id="d8b7a-103">Det kan vara att när du öppnar filer öppnas i skrivskyddat läge.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="d8b7a-104">I vissa fall är detta för extra säkerhet som när du öppnar filer från internet och andra tillfällen då det kan bero på en inställning som kan ändras.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="d8b7a-105">Här följer några scenarier där en fil öppnas skrivskyddat och några åtgärder som du kan ändra som.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="d8b7a-106">**Mitt antivirusprogram orsakar dem skrivskyddad**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="d8b7a-107">Vissa antivirusprogram kan skydda dig mot eventuellt osäkra filer genom att öppna dem som skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="d8b7a-108">Du kan behöva kontakta leverantören av antivirusprogrammet för information om hur du ändrar de här inställningarna.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="d8b7a-109">BitDefender, till exempel har innehåll att lägga till här programundantag: [hur du lägger till programmet eller processen undantag i Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="d8b7a-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="d8b7a-110">**Egenskaperna anges skrivskyddat?**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="d8b7a-111">Du kan kontrollera egenskaperna genom att högerklicka på filen och välja egenskaper.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="d8b7a-112">Om det skrivskyddade attributet är markerat kan du avmarkera den och på OK.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="d8b7a-113">**Innehållet är i skyddad vy**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="d8b7a-114">Filer från Internet och andra potentiellt osäkra platser kan innehålla virus, maskar och andra typer av skadlig kod som kan skada din dator.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="d8b7a-115">Detta gäller även ofta med bifogade filer eller filer som du har hämtat.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="d8b7a-116">Om du vill skydda datorn öppnas filer från dessa potentiellt osäkra platser i skyddad vy.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="d8b7a-117">Du kan läsa en fil och se innehållet samtidigt som det minskar riskerna med hjälp av skyddad vy.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="d8b7a-118">Mer information om skyddad vy och hur du ändrar inställningarna läser du följande artikel: [Vad är skyddad vy?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="d8b7a-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="d8b7a-119">**Är OneDrive full?**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="d8b7a-120">Om filen lagras på OneDrive och OneDrive-lagringsutrymme är full, du inte spara dokumentet tills du är under din tilldelat utrymme.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="d8b7a-121">Du kan kontrollera ditt utrymme på OneDrive genom att klicka på ikonen för OneDrive i mitt meddelande hantera lagring eller går du till [http://onedrive.live.com](http://onedrive.live.com), logga in och Observera mängden utrymme längst ned till vänster på skärmen.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="d8b7a-122">**Är aktiverat för Office**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="d8b7a-123">Om Office inte är aktiverad, eller om din prenumeration har gått ut, kan du vara i skrivskyddat läge läget Nedsatt funktionalitet.</span><span class="sxs-lookup"><span data-stu-id="d8b7a-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="d8b7a-124">Mer information om hur du aktiverar Office finns: [Ej licensierad produkt och Aktiveringsfel i Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="d8b7a-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="d8b7a-125">**Om allt annat misslyckas...**</span><span class="sxs-lookup"><span data-stu-id="d8b7a-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="d8b7a-126">Försök att starta om datorn</span><span class="sxs-lookup"><span data-stu-id="d8b7a-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="d8b7a-127">Installera Office-uppdateringar</span><span class="sxs-lookup"><span data-stu-id="d8b7a-127">Install Office updates</span></span>
    
- <span data-ttu-id="d8b7a-128">En Online reparation av Office</span><span class="sxs-lookup"><span data-stu-id="d8b7a-128">Perform an Online repair of Office</span></span>
    

