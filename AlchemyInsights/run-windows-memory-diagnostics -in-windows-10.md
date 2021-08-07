---
title: Kör Windows minnesdiagnostik i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922589"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Kör Windows minnesdiagnostik i Windows 10

Om Windows appar på datorn kraschar, fryser eller fungerar instabilt kan du ha problem med datorns minne . Du kan köra Windows minnesdiagnostik för att söka efter problem med datorns RAM-minne.

Skriv minnesdiagnostik i sökrutan i **Aktivitetsfältet** och välj sedan Ta **Windows minnesdiagnostik.** 

För att kunna köra diagnostiken måste datorn starta om. Du kan starta om direkt (spara ditt arbete och stäng öppna dokument och e-postmeddelanden först) eller schemalägga diagnostiken så att den körs automatiskt nästa gång datorn startar om:

![Windows Minnesdiagnostik](media/windows-memory-diagnostic.png)

När datorn startas om körs **Windows minnesdiagnostikverktyget** automatiskt. Status och förlopp visas medan diagnostiken körs och du kan välja att avbryta diagnostiken genom att trycka på **ESC** på tangentbordet.

När diagnostiken är klar Windows startar den normalt.
Omedelbart efter omstarten, när skrivbordet visas, visas  ett meddelande (bredvid ikonen för Åtgärdscenter i Aktivitetsfältet) som anger om några minnesfel hittades. Till exempel:

Här är ikonen för Åtgärdscenter: ![Ikon för Åtgärdscenter](media/action-center-icon.png) 

Och ett exempelmeddelande: ![Inga minnesfel](media/no-memory-errors.png)

Om du missade meddelandet kan  du välja ikonen för Åtgärdscenter i Aktivitetsfältet för att visa **Åtgärdscenter** och se en rullningsbar lista med meddelanden.

Om du vill granska detaljerad information **skriver** du händelsen i sökrutan i Aktivitetsfältet och väljer sedan **Loggboken**. I det **vänstra fönstret** i loggboken går du till fönstret Windows loggar **> System**. I fönstret till höger söker du nedåt i  listan medan du tittar på kolumnen Källa, tills du ser händelser med källvärdet **Minnesdiagnostics-Resultat.** Markera varje sådan händelse och se resultatinformationen i rutan under **fliken** Allmänt under listan.
