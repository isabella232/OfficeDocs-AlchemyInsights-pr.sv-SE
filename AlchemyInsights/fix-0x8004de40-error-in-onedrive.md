---
title: Åtgärda 0x8004de40 i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649766"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Åtgärda 0x8004de40 i OneDrive

Om du kör Windows 7 och får det här felet, uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.

Om du kör Windows 10 och du får ett meddelande om 0x8004de40 med OneDrive:

- Starta om den dator som påverkas när du är ansluten till din Acitve-katalogdomän.
- Om en omstart inte löser problemet kan du ta bort och återansluta till enheten från Azure AD. 

**Obs!** Du bör vara i företagets nätverk när du utför de här stegen. Utför inte de här stegen när du inte är ansluten till företagets infrastruktur (till exempel när du reser). 

1. Öppna en upphöjd kommandotolk genom **att välja Start**, högerklicka på **Kommandotolken** och välj **sedan Kör som administratör.**

1. Skriv *dsregcmd /leave och* tryck på **Retur.**

1. När du är klar skriver *du dsregcmd /join* och trycker på **Retur.**

1. Stäng kommandotolken när du är klar.

1. Starta om datorn och logga in på OneDrive.