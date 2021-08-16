---
title: Exempel på en princip för bifogad fil Office 365 Valv Microsoft Defender för företag
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988313"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exempel på en princip för bifogad fil Office 365 Valv Microsoft Defender för företag

De här inställningarna aktiverar principen *No delays* (Inga fördröjningar) som skickar meddelanden direkt och sedan återansluter bifogade filer när de har skannats:

- **Namn**: Inga fördröjningar
- **Beskrivning**: Levererar meddelanden omedelbart ochbibiar bifogade filer efter genomsökning.
- **Svar:** Välj **alternativet Dynamisk** leverans. Mer information finns i Principer [för dynamisk leverans i Valv för bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Avsnittet Omdirigera bifogad** fil: Välj alternativet Aktivera omdirigering och ange sedan e-postadressen till din globala Microsoft 365-administratör, säkerhetsadministratör eller säkerhetsanalytiker som ska undersöka skadliga bifogade filer. 
- **Avsnittet Används** för: **Välj Mottagarens domän är** och välj sedan din domän. Välj **lägg** till och välj sedan **OK.** Välj Spara när du är **klar.**

Mer information finns i Lägga [Valv i Microsoft Defender för Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
