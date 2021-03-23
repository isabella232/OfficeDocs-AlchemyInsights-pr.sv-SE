---
title: Frigöra diskutrymme i Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037950"
---
# <a name="free-up-drive-space-in-windows-10"></a>Frigöra diskutrymme i Windows 10

Här är två alternativ för att frigöra diskutrymme i Windows:

- Frigör diskutrymme i Windows 10.
- Frigör utrymme för Windows 10-uppdateringar med extern lagringsenhet.

Om du fortfarande har låg diskutrymme efter att ha använt Diskrensning är det möjligt att Temp-mappen snabbt fylls upp med programfiler (.appx) som används av Microsoft Store. Lös problemet genom att återställa Store, rensa Store-cachen och sedan köra Felsökaren för Windows Update. Se till att Microsoft Store är stängt innan du fortsätter med de här stegen.

**Steg 1: Återställ Microsoft Store**

**Obs!** Då tas appdata på enheten bort permanent, inklusive dina inställningar och inloggningsuppgifter.

1. Välj **Starta**  >  **inställningar**  >  **Appar**  >  **& funktioner**.

1. Leta reda på och välj Microsoft Store i listan med appar.

1. Välj **Avancerade alternativ**.

1. Rulla nedåt och välj **Återställ** och sedan **Bekräfta återställning.**

**Steg 2: Rensa Microsoft Store-cachen**

1. Tryck på Windows-tangenten + R för att öppna dialogrutan Kör.

1. Skriv wsreset.exe och välj **OK**.

1. Ett tomt kommandotolkfönster öppnas. Efter ungefär 10 sekunder stängs fönstret och Store öppnas automatiskt.

**Steg 3: Återställ Windows Update**

1. Välj **Starta**  >  **inställningar**  >  **Uppdatering &**  >  **säkerhetsfelsök**.

1. Rulla nedåt och **välj Windows Update** i listan och välj Kör **felsökaren**.

1. Starta om datorn och kontrollera om du fortfarande upplever problemet.

