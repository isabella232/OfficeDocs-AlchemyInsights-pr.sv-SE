---
title: Korrigera fel i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133994"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Korrigera fel i 0x8004de40 i OneDrive

Om du får felmeddelandet 0x8004de40 med OneDrive:

- Starta om datorn när du är ansluten till akitv Directory-domän.
- Om en omstart inte löser problemet, koppla från och återansluta enheten från Azure AD. 

**Obs**: du bör vara på företagets nätverk när du utför dessa steg. Inte utföra dessa steg när du inte kan ansluta till ditt företags infrastruktur (t.ex, under resa). 

- Öppna en kommandotolk. 
- Öppna en kommandotolk Klicka på - **Start**, högerklicka på **Kommandotolken**och klicka sedan på **Kör som administratör**.
- *Dsregcmd /leave* och tryck på **RETUR**.
- När du är klar, *dsregcmd, /join* och tryck på **RETUR**.
- Stäng Kommandotolken när du är färdig.
- Starta om datorn och logga in på OneDrive.