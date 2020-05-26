---
title: Köra Windows Minnesdiagnostik i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358293"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Köra Windows Minnesdiagnostik i Windows 10

Om Windows och appar på datorn kraschar, fryser eller agerar på ett instabilt sätt kan det vara problem med datorns minne (RAM). Du kan köra Windows Memory Diagnostic för att söka efter problem med datorns RAM.You can run the Windows Memory Diagnostic to check for problems with the PC's RAM.

Skriv **minnesdiagnostik**i sökrutan i Aktivitetsfältet och välj sedan **Windows Minnesdiagnostik**. 

För att köra diagnostiken måste datorn startas om. Du har möjlighet att starta om omedelbart (spara ditt arbete och stäng öppna dokument och e-post först), eller schemalägga diagnostiken så att den körs automatiskt nästa gång datorn startas om:

![Diagnostik av Windows-minne](media/windows-memory-diagnostic.png)

När datorn startas om körs **Windows Minnesdiagnostikverktyg** automatiskt. Status och förlopp visas när diagnostiken körs, och du har möjlighet att avbryta diagnostiken genom att trycka på **ESC-tangenten** på tangentbordet.

När diagnostiken är klar startar Windows normalt.
Omedelbart efter omstarten visas ett meddelande (bredvid **åtgärdscenterikonen** i Aktivitetsfältet) när skrivbordet visas (bredvid åtgärdscenterikonen i Aktivitetsfältet) för att ange om några minnesfel hittades. Ett exempel:

Här är ikonen i Åtgärdscenter: ![Ikon för Åtgärdscenter](media/action-center-icon.png) 

Och ett exempel meddelande: ![Inga minnesfel](media/no-memory-errors.png)

Om du missade meddelandet kan du välja **ikonen Åtgärdscenter** i Aktivitetsfältet för att visa **Åtgärdscenter** och se en rullningsbar lista med meddelanden.

Om du vill granska detaljerad information skriver du **händelsen** i sökrutan i Aktivitetsfältet och väljer sedan **Loggboken**. I **loggbokens**vänstra fönster navigerar du till **Windows-loggar > System**. I det högra fönstret söker du ned listan medan du tittar på kolumnen **Källa** tills du ser händelser med källvärde **Minnesdiagnostik-resultat**. Markera varje sådan händelse och se resultatinformationen i rutan under fliken **Allmänt** under listan.
