---
title: 0x8004de40 vid start av OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813670"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="164b9-102">0x8004de40 vid start av OneDrive</span><span class="sxs-lookup"><span data-stu-id="164b9-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="164b9-103">Om ett felmeddelande visas när **0x8004de40** loggar in på OneDrive startar du om datorn medan du är ansluten till din arbets- eller skoldomän.</span><span class="sxs-lookup"><span data-stu-id="164b9-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="164b9-104">Om det här felmeddelandet visas när du har startat om kan du försöka med det här när du är ansluten till din arbets- eller skoldomän:</span><span class="sxs-lookup"><span data-stu-id="164b9-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="164b9-105">Klicka på Start och skriv **cmd** eller **kommandotolken** i sökrutan, högerklicka på kommandotolken och välj **Kör som administratör.**</span><span class="sxs-lookup"><span data-stu-id="164b9-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="164b9-106">Om du uppmanas att ange ett administratörslösenord eller att bekräfta skriver du lösenordet eller klickar på **Tillåt**.</span><span class="sxs-lookup"><span data-stu-id="164b9-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="164b9-107">I fönstret Kommandotolken skriver du **dsregcmd /leave**  och väntar tills kommandot har slutförts.</span><span class="sxs-lookup"><span data-stu-id="164b9-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="164b9-108">Skriv **sedan dsregcmd /join** och vänta tills kommandot har slutförts.</span><span class="sxs-lookup"><span data-stu-id="164b9-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="164b9-109">Starta om datorn.</span><span class="sxs-lookup"><span data-stu-id="164b9-109">Reboot your computer.</span></span>
