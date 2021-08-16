---
title: Installera Office och OneDrive på Windows virtuellt skrivbord
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
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028634"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installera Office och OneDrive på Windows virtuellt skrivbord

1. [Förbereda och anpassa en MALL-VHD-bild](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Skapa en virtuell dator (VM) om den inte redan har skapats.

1. [Installera Office i läget för aktivering på delad dator.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivering på delad dator ger flera användare åtkomst till Office.

1. [Installera OneDrive i per datorläge](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Normalt sett OneDrive per användare, men här ska det installeras per dator.