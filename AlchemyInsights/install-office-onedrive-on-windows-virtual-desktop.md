---
title: Installera Office och OneDrive på virtuellt skrivbord i Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596032"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="9f1f3-102">Installera Office och OneDrive på virtuellt skrivbord i Windows</span><span class="sxs-lookup"><span data-stu-id="9f1f3-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="9f1f3-103">[Förbereda och anpassa en MALL-VHD-bild](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="9f1f3-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="9f1f3-104">Skapa en virtuell dator (VM) om den inte redan har skapats.</span><span class="sxs-lookup"><span data-stu-id="9f1f3-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="9f1f3-105">[Installera Office i aktiveringsläge för delad dator](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span><span class="sxs-lookup"><span data-stu-id="9f1f3-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="9f1f3-106">Aktivering på delad dator ger flera användare åtkomst till Office.</span><span class="sxs-lookup"><span data-stu-id="9f1f3-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="9f1f3-107">[Installera OneDrive i per datorläge](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span><span class="sxs-lookup"><span data-stu-id="9f1f3-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="9f1f3-108">Normalt installeras OneDrive per användare, men här ska det installeras per dator.</span><span class="sxs-lookup"><span data-stu-id="9f1f3-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>