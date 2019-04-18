---
title: Identifiera delete message händelser i granskningsloggar
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909601"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Granska loggarna för borttagna e-postmeddelanden

Börjar i januari 2019 Microsoft aktivera postlådan Granskningsloggningen som standard. Annars, om du vill granska händelser för ta bort meddelande för en viss användare, måste du aktivera manuellt ta bort åtgärder för granskning. Om postlådan granska loggning är redan aktiverat för organisationen eller för specifika användare, följer du stegen nedan.

1. Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)

2. Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.

3. Välj datumintervall i fälten **startdatum** och **slutdatum** . Ange användarnamnet för den användare som du vill undersöka (användare som borttagna objekt). Välj i fältet **verksamhet** **borttagna meddelanden från mappen Borttaget** och **Moved meddelanden till mappen Borttaget**.

4. Klicka på **Sök**.

Markera en granskningspost i resultatet. Klicka på **Mer Information**i information-utfällbar. Ytterligare information om det borttagna objektet (till exempel ämnesraden och placeringen av objektet när den togs bort) visas i fältet **AffectedItems** . Egenskapen **ClientInfoString** visas om borttagningen uppstod i Outlook, Outlook på webben (kallades tidigare Outlook Web App) eller någon annan enhet.

Mer information finns i [fastställa som definierar e-vidarebefordran för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Obs**: du kan inte hämta borttagna objekt med hjälp av funktionen Granska loggen. Om du vill återställa borttagna meddelanden i Outlook på webben finns i [Återskapa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
