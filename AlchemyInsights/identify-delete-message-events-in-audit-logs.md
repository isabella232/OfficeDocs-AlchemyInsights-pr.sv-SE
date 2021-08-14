---
title: Identifiera borttagningsmeddelandehändelser i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868436"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Granskningsloggar för borttagna e-postmeddelanden

Från och med januari 2019 startar Microsoft granskningsloggning för postlådor som standard. Annars måste du manuellt aktivera borttagningsåtgärder för granskning om du vill granska borttagningshändelser för en viss användare. Om granskningsloggning för postlådor redan är aktiverad för organisationen eller för en viss användare följer du stegen nedan.

1. Logga in på [Microsoft 365 Säkerhets- och efterlevnadscenter](https://protection.office.com/)

2. Klicka **på Sökning och undersökning** och välj **Granskningsloggsökning**.

3. Välj datumintervallet i **fälten Startdatum** **och** Slutdatum. Ange användarnamn för den användare som du vill undersöka (den användare som tog bort objekten). I fältet **Aktiviteter** väljer du **Borttaget från mappen Borttaget och** **Flyttade meddelanden till mappen Borttaget.**

4. Klicka **på Sök**.

Välj en granskningspost i resultatet. Klicka på Mer information i den **utfällade informationen.** Ytterligare information om det borttagna objektet (till exempel ämnesraden och platsen för objektet när det togs bort) visas i **fältet AffectedItems.** Egenskapen **ClientInfoString** visar om borttagningen inträffade på Outlook, Outlook på webben (tidigare kallad Outlook Web App) eller någon annan enhet.

Mer information finns i Fastställa [vem som har konfigurerat vidarebefordran av e-post för en postlåda.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Obs!** Du kan inte hämta borttagna objekt med hjälp av granskningsloggfunktionen. Information om hur du hämtar borttagna Outlook på webben meddelanden finns [i Återskapa borttagna objekt i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
