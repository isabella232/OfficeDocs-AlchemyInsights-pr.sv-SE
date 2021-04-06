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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installera Office och OneDrive på virtuellt skrivbord i Windows

1. [Förbereda och anpassa en MALL-VHD-bild](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Skapa en virtuell dator (VM) om den inte redan har skapats.

1. [Installera Office i aktiveringsläge för delad dator](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Aktivering på delad dator ger flera användare åtkomst till Office.

1. [Installera OneDrive i per datorläge](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalt installeras OneDrive per användare, men här ska det installeras per dator.