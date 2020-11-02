---
title: 0x8004de40-fel när du startar OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823119"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="6d722-102">0x8004de40-fel när du startar OneDrive</span><span class="sxs-lookup"><span data-stu-id="6d722-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="6d722-103">Om du får ett fel **meddelande när du** loggar in på OneDrive startar du om datorn när du är ansluten till din arbets-eller skol domän.</span><span class="sxs-lookup"><span data-stu-id="6d722-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="6d722-104">Om du får det här felet efter att du har startat om datorn kan du prova det när du är ansluten till din arbets-eller skol domän:</span><span class="sxs-lookup"><span data-stu-id="6d722-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="6d722-105">Klicka på Start och skriv **cmd** eller **kommando tolken**  i sökrutan, högerklicka på appen kommando tolken och välj  **Kör som administratör** .</span><span class="sxs-lookup"><span data-stu-id="6d722-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="6d722-106">Om du uppmanas att ange ett administratörs lösen ord eller en bekräftelse skriver du lösen ordet eller klickar på **Tillåt** .</span><span class="sxs-lookup"><span data-stu-id="6d722-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="6d722-107">I kommando tolken skriver du **dsregcmd/Leave**  och väntar på att kommandot ska slutföras.</span><span class="sxs-lookup"><span data-stu-id="6d722-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="6d722-108">Skriv sedan **dsregcmd/Join** och vänta tills kommandot har slutförts.</span><span class="sxs-lookup"><span data-stu-id="6d722-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="6d722-109">Starta om datorn.</span><span class="sxs-lookup"><span data-stu-id="6d722-109">Reboot your computer.</span></span>
