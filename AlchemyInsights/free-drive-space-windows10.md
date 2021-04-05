---
title: Frigör diskutrymme i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505374"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frigör diskutrymme i Windows 10

Här är två alternativ för att frigöra diskutrymme i Windows:

- Frigör diskutrymme i Windows 10.
- Frigör utrymme för Windows 10-uppdateringar med en extern lagringsenhet.

Om du fortfarande har låg diskutrymme efter att du har använt Diskrensning är det möjligt att Temp-mappen snabbt fylls på med programfiler (.appx) som används i Microsoft Store. Lös problemet genom att återställa Store, rensa Store-cachen och kör sedan felsökaren för Windows Update. Kontrollera att Microsoft Store är stängt innan du fortsätter med de här stegen.

**Steg 1: Återställ Microsoft Store**

**Obs** Detta tar bort appdata på enheten permanent, inklusive dina inställningar och inloggningsuppgifter.

1. Välj **Start** > **Inställningar** > **Appar** > **Appar och funktioner**.

1. Leta reda på och välj Microsoft Store i listan med program.

1. Välj **Avancerade alternativ**.

1. Rulla nedåt och välj **Återställa** och välj sedan **Bekräfta återställa**.

**Steg 2: Rensa Microsoft Store-cachen**

1. Tryck på Windows-tangenten+R för att öppna dialogrutan Kör.

1. Skriv wsreset.exe och välj **OK**.

1. Ett tomt Kommandotolkens fönster öppnas. Efter ungefär 10 sekunder stängs fönstret och Store öppnas automatiskt.

**Steg 3: Återställa Windows Update**

1. Välj **Start** > **Inställningar** > **Uppdatera och Säkerhet** > **Felsöka**.

1. Rulla nedåt och välj **Windows Update** i listan och välj **Kör felsökaren**.

1. Starta om datorn och kontrollera om du fortfarande har det här problemet.

