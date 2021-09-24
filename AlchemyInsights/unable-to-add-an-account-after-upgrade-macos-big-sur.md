---
title: Det går inte att lägga till ett konto efter uppgradering till macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506758"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Det går inte att lägga till ett konto efter uppgradering till macOS 11.6 Big Sur

När du uppgraderat till macOS 11.6 kanske ditt OneDrive för arbets- eller skolkonto eller ditt personliga OneDrive-konto inte visas i listan med konton och du kanske inte kan logga in på ett andra konto från appen.

En korrigering har utvecklats för det här problemet. Kontrollera först om du kör den fristående versionen eller App Store-versionen OneDrive:

- Välj OneDrive i menyraden och klicka > **i & Inställningar**  >  **Inställningar**  >  **om**. Om versionsnumret inte innehåller **(fristående) har** du App Store-versionen av produkten.

Om du använder den fristående versionen av OneDrive du om datorn och OneDrive till en version där problemet är löst. Om du vill installera versionen manuellt laddar du ned den [här.zip-filen](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), packa upp filen och kopierar OneDrive-appen till mappen Program (genom att ersätta den befintliga OneDrive-appen).

Om du använder App Store-versionen kan det vara bra att installera den fristående versionen av OneDrive. Den här versionen fungerar på samma sätt som App Store-versionen men gör att Microsoft kan erbjuda uppdateringar snabbare för användare och ansluta dem till en version som innehåller korrigeringen för det här problemet.

1. Ladda ned den fristående versionen [OneDrive som innehåller korrigeringen](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Packa upp filen och kopiera den OneDrive till mappen Program (genom att ersätta den befintliga OneDrive appen).

Om du behöver använda App Store-versionen väntar du tills App Store släpper en version av appen som innehåller korrigeringen. Tyvärr kan Microsoft inte meddela ett beräknat datum för att en fast version ska släppas från App Store.


