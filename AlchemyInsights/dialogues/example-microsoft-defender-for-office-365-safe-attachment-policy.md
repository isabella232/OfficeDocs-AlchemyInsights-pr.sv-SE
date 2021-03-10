---
title: Exempel på princip för Säker bifogad fil i Microsoft Defender för Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695187"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exempel på princip för Säker bifogad fil i Microsoft Defender för Office 365

De här inställningarna aktiverar principen *Inga fördröjningar* som levererar meddelanden omedelbart och sedan bifogar bifogade filer igen när de skannas:

- **Namn:** Inga fördröjningar
- **Beskrivning:** Levererar meddelanden omedelbart och bifogar bifogade filer igen efter genomsökning.
- **Svar:** Välj **alternativet Dynamisk** leverans. Mer information finns i principer [för dynamisk leverans i principer för säkra bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Avsnittet Omdirigering** av bifogade filer: Välj alternativet för att aktivera omdirigering och ange sedan e-postadressen till din globala Microsoft 365-administratör, säkerhetsadministratör eller säkerhetsanalytiker som undersöker skadliga bifogade filer.
- **Avsnittet Tillämpas** på: **Välj mottagarens domän** är, och välj sedan din domän. Välj **Lägg till** och välj sedan **OK.** Välj Spara när du är **klar.**

Mer information finns i Säkra [bifogade filer i Microsoft Defender för Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
