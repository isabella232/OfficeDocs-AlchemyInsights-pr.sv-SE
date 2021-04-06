---
title: Verktyget Tjänstdiagnostik för Windows Virtual Desktop
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
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596046"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Verktyget Tjänstdiagnostik för Windows Virtual Desktop

Windows Virtual Desktop (WVD) innehåller ett diagnostikverktyg som gör att administratörer kan identifiera fel i ett enda gränssnitt. Det här verktyget loggar diagnosrelaterad information när WVD används av någon som tilldelats en WVD-roll. Varje logg innehåller information om WVD-rollen som ingår i aktiviteten, felmeddelanden som visas under sessionen och information om klientorganisationen och användaren. Azure-logganalys kan konfigureras för att registrera aktivitetsloggen som skapats av diagnostikverktyget genom att följa de här stegen:

1. Skapa en arbetsyta för logganalys med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) [eller Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Anslut Windows-datorer till Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Hämta Arbetsyte-ID och primärnyckel för arbetsytan. Installationsguiden behöver den här informationen för att kunna konfigurera agenten på rätt sätt och för att säkerställa att den kan kommunicera med Azure Monitor.

1. [Skicka diagnostikdata till arbetsytan](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan push-diagnostikdata från WVD-klienten till logganalysen för arbetsytan.

1. [Identifiera och diagnostisera](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problem som är interna eller externa i relation till WVD.

Mer information om hur du konfigurerar tjänstdiagnostikverktyget för WVD finns i Använda logganalys för diagnostikfunktionen.