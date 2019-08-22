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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525077"
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