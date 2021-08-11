---
title: Läsa granskningsloggarna för borttagna händelser
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967351"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Läsa granskningsloggarna för borttagna händelser

Gör så här:

1. Gå till [säkerhets- Office 365 för & säkerhets- och efterlevnadscenter.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök i**  >  [**granskningsloggsökning**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Om du ser att du måste aktivera funktionen kan du aktivera den nu. Om funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Välj **Aktiviteter** och leta upp Exchange **postlådeaktiviteter.** Välj alternativen **Borttaget från mappen Borttaget** och Flyttade meddelanden till mappen **Borttaget.** När du är klar klickar du utanför fönstret för att minimera **fönstret** Aktiviteter.
1. Ange datumintervallet och välj sedan **användarnamnet** för den användare du vill undersöka i rutan Användare. Du kan välja fler än en användare i taget.
1. Välj **Sök**. Aktiviteterna visas under **Resultat.**
1. Om du vill visa informationen väljer du en aktivitet och sedan **Mer information**. Mer information om det borttagna objektet, till exempel ämnesraden och platsen för objektet när det togs bort, visas i **fältet AffectedItems.**
    > [!NOTE]
    > Du kan inte återställa borttagna objekt med granskningsloggfunktionen. Information om hur du återställer borttagna objekt [finns i Återskapa borttagna objekt eller e-Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Mer information finns i Söka [i Office 365 granskningsloggen för att felsöka vanliga scenarier](https://go.microsoft.com/fwlink/?linkid=2103944).
