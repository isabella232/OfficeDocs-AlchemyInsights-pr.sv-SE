---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716046"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Åtgärda 0x8004de40-fel i OneDrive

Om du får ett 0x8004de40-fel med OneDrive:

- Starta om den dator som påverkas när den är ansluten till Acitve Directory-domänen.
- Om en omstart inte löser problemet kan du koppla bort och ansluta till enheten från Azure AD igen. 

**Du**bör vara i företagets nätverk när du utför dessa steg. Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser). 

- Öppna en upphöjd kommandotolk. 
- Om du vill öppna en upphöjd kommandotolk klickar du på - **Starta**, högerklickar på **Kommandotolken**och klickar sedan på **Kör som administratör**.
- Skriv *dsregcmd /leave* och tryck på **Retur**.
- När du är klar skriver du *dsregcmd /join* och trycker på **Retur**.
- När du är klar stänger du kommandotolken.
- Starta om datorn och logga in på OneDrive.