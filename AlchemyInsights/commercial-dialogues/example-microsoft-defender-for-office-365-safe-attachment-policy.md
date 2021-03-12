---
title: Exempel på princip för säkra bifogade filer i Microsoft Defender för Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749195"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Exempel på princip för säkra bifogade filer i Microsoft Defender för Office 365

De här inställningarna aktiverar principen *No delays* (Inga fördröjningar) som skickar meddelanden direkt och sedan återansluter bifogade filer när de har skannats:

- **Namn**: Inga fördröjningar
- **Beskrivning**: Levererar meddelanden omedelbart ochbibiar bifogade filer efter genomsökning.
- **Svar:** Välj **alternativet Dynamisk** leverans. Mer information finns i Principer [för dynamisk leverans i säkra bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Avsnittet Omdirigera bifogad** fil: Välj alternativet Aktivera omdirigering och ange sedan e-postadressen till din globala Microsoft 365-administratör, säkerhetsadministratör eller säkerhetsanalytiker som ska undersöka skadliga bifogade filer. 
- **Avsnittet Används** för: **Välj Mottagarens domän är** och välj sedan din domän. Välj **lägg** till och välj sedan **OK.** Välj Spara när du är **klar.**

Mer information finns i Säkra [bifogade filer i Microsoft Defender för Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
