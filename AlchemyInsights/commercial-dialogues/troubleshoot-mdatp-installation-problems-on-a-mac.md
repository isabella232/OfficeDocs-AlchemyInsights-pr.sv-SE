---
title: Felsöka problem med MDATP-installationen på en Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749767"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Felsöka problem med MDATP-installationen på en Mac

Om manuell installation misslyckas **visas** följande fel på sidan Sammanfattning av installationsguiden:

"Ett fel uppstod under installationen. Installationsprogrammet påträffade ett fel som orsakade att installationen misslyckades. Kontakta programvarutillverkaren för att få hjälp."

För MDM-distributioner visar sidan också ett allmänt installationsfel.

Även om vi inte visar exakta fel för slutanvändare så sparar vi en loggfil med installationsstatus i **/Bibliotek/Loggar/Microsoft/mdatp/install.log.** Varje installationssession läggs till i den här loggfilen. Om du bara vill mata ut den senaste installationssessionen använder du `sed` .

Mer information finns i [Felsöka installationsproblem för Microsoft Defender ATP för Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
