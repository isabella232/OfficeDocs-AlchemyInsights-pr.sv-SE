---
title: Använda TeamViewer för att fjärrdministrera Intune-enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555751"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Använda TeamViewer för att fjärrdministrera Intune-enheter

Enheter som hanteras av Intune kan fjärrges med [TeamViewer](https://www.teamviewer.com/).

Så här administrerar du Intune med TeamViewer: 

Börja med att hämta autentiseringsuppgifter från TeamViewer för att konfigurera TeamViewer Connector på Intune. På så sätt kan administratören ange autentiseringsuppgifter i TeamViewer Connector-användargränssnittet under Enheter, en engångsåtgärd för att upprätta länken mellan Intune och TeamViewer-tjänsten.

**Del 1: Starta en session med en fjärrenhet**

1. Under **Alla enheter**väljer du den enhet som du vill starta en fjärrsession med.
2. Från **... Mer**väljer du **Ny fjärrhjälpssession**.
3. Välj **Ja** för att bekräfta att du vill upprätta en fjärrsession.
    När begäran om att initiera en ny fjärrsession har bekräftats av TeamViewer-tjänsten visas ett alternativ för att **starta fjärrhjälp** under information om fönstret Översikt (eller Essentials) för enheten. Välj **Visa mer** om du vill expandera fönstret och visa fjärrhjälpsstatus.
4. Välj **Starta fjärrsession** om du vill starta sessionen på administratörssidan.
5. Välj att hämta Den binära TeamViewer (Windows) och välj **Kör**.<br/>
    **Anm.)** Du kan ignorera alla webbläsar sidor öppnas till TeamViewer webbplats.

6. Bekräfta begäran om att TeamViewer-appen ska göra ändringar på enheten (endast Windows).
7. TeamViewer-appen startar och innehåller sessionskoden för att autentisera anslutningen med fjärrenheten.

**Del 2: På den enhet som är avsedd för en fjärrsession**

1. Öppna Företagsportalen Intune.
2. Leta efter en aviseringsflagga: "IT-administratören begär kontroll över den här enheten för en fjärrhjälpssession" och väljer meddelandet.
3. Välj att ladda ned TeamViewer-programmet eller bekräfta nedladdningen av TeamViewer-appen från App Store och välj **Kör**.
    **Anm.)** Du kan ignorera alla webbläsar sidor öppnas till TeamViewer webbplats.

4. Bekräfta begäran om att TeamViewer-appen ska göra ändringar på enheten (endast Windows).
5. TeamViewer-appen startar och innehåller sessionskoden för att autentisera anslutningen med fjärrenheten.
6. En popup frågar om du vill tillåta sessionen att starta.

**Anm.)** De sessionskoder som genereras av TeamViewer-tjänsten används endast en gång. Om du förlorar anslutningen måste du:

1. Stäng instansen av TeamViewer-appen på fjärrenheten och på administratörsarbetsstationen.
2. Stäng företagsportalen på fjärrenheten.
3. Starta en ny "Ny fjärrhjälpssession" från administratörsportalen.
4. Öppna företagsportalen på fjärrenheten igen för att ta emot det nya meddelandet.
5. Ladda ned och öppna TeamViewer-appen på både fjärrenheten och administratörsarbetsstationen, som tidigare.