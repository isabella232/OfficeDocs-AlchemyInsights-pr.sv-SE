---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755866"
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