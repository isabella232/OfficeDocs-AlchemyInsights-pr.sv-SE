---
title: Identifiera borttagning av meddelandehändelser i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509006"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Granskningsloggar för borttagna e-postmeddelanden

Från och med januari 2019 aktiverar Microsoft loggning av postlådor som standard. Om du vill granska borttagningshändelser för en viss användare måste du aktivera borttagningsåtgärderna manuellt för granskning. Om loggning av postlådor redan är aktiverat för din organisation eller för den specifika användaren följer du stegen nedan.

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klicka på **Sök och utredning** och välj **Granskningsloggsökning**.

3. Välj datumintervall i fälten **Startdatum** och **Slutdatum.** Ange användarnamn för den användare som du vill undersöka (användaren som tog bort objekten). I fältet **Aktiviteter** väljer du **Borttagna meddelanden från mappen Borttaget** och **Flyttade meddelanden till mappen Borttaget.**

4. Klicka på **Sök**.

Välj en granskningspost i resultatet. Klicka på **Mer information**i informationsutfällbara. Ytterligare information om det borttagna objektet (till exempel ämnesraden och platsen för objektet när det togs bort) visas i fältet **AffectedItems.** Egenskapen **ClientInfoString** visas om borttagningen inträffade i Outlook, Outlook på webben (tidigare kallat Outlook Web App) eller någon annan enhet.

Mer information finns i [Bestämma vem som konfigurerar vidarebefordran av e-post för en postlåda](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Du**kan inte hämta borttagna objekt med hjälp av granskningsloggfunktionen. Information om hur du hämtar borttagna meddelanden i Outlook på webben finns [i Återställa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
