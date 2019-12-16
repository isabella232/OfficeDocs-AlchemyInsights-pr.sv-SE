---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052055"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Åtgärda 0x8004de40-fel i OneDrive

Om du får ett 0x8004de40-fel med OneDrive:

- Starta om den aktuella datorn när du är ansluten till din Acitve Directory-domän.
- Om en omstart inte löser problemet, ta bort kopplingen och Anslut din enhet från Azure AD. 

**Du bör**vara i företagsnätverket när du utför dessa steg. Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser). 

- Öppna en upphöjd kommandotolk. 
- Om du vill öppna en upphöjd kommandotolk klickar du på **Start**, högerklickar på **Kommandotolken**och klickar sedan på **Kör som administratör**.
- Skriv *dsregcmd/Leave* och tryck på **RETUR**.
- När du är klar skriver du *dsregcmd/Join* och trycker på **RETUR**.
- Stäng Kommandotolken när du är klar.
- Starta om datorn och logga in på OneDrive.