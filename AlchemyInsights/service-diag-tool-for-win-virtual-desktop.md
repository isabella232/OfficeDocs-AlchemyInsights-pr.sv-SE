---
title: Service Diagnostics Tool för Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680233"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service Diagnostics Tool för Windows Virtual Desktop

Windows Virtual Desktop (WVD) erbjuder ett diagnostikverktyg som låter administratörer identifiera fel genom ett enda gränssnitt. Det här verktyget loggar diagnostikinformation-relaterad information när WVD används av någon som tilldelats en WVD-roll. Varje logg innehåller information om den WVD rollen som är involverad i aktiviteten, de fel meddelanden som visas under sessionen samt uppgifter om klient organisationen och användaren. Azure Log Analytics kan konfigureras för att fånga in aktivitets loggen som skapas av diagnostikverktyget. Så här gör du:

1. Skapa en logganalys-arbetsyta med [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Anslut Windows-datorer till Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Hämta arbetsyte-ID och primärt för arbets ytan. Installations guiden behöver den här informationen för att konfigurera agenten på rätt sätt och för att säkerställa att den kan kommunicera med Azure Monitor.
1. [Pusha diagnostikdata till din arbets yta](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan skicka diagnos data från din WVD-klient till logg analys för arbets ytan.
1. [Identifiera och diagnostisera problem](https://go.microsoft.com/fwlink/?linkid=2128338) som är interna eller externa i relation till WVD.

Mer information om hur du konfigurerar verktyget för WVD finns i [använda logg analys för funktionen diagnostik](https://go.microsoft.com/fwlink/?linkid=2128084).
