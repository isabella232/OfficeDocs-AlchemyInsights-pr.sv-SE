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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429821"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Läsa granskningsloggarna för borttagna händelser

Gör så här:

1. Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök**  >  [**granskningsloggsökning.**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera funktionen kan du aktivera den nu. Om funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Välj **Aktiviteter** och sök sedan efter **aktiviteter i Exchange-postlådan.** Välj **borttagna meddelanden från mappen Borttaget** och **flyttade meddelanden till mappalternativen Borttaget.** När du är klar klickar du utanför fönstret för att minimera **fönstret** Aktiviteter.
1. Ange datumintervallet och välj sedan **användarnamnet** för den användare du vill undersöka i rutan Användare. Du kan välja flera användare åt gången.
1. Välj **Sök.** Aktiviteterna visas under **Resultat.**
1. Om du vill visa informationen väljer du en aktivitet och sedan **Mer information.** Mer information om det borttagna objektet, till exempel ämnesraden och objektets plats när det togs bort, visas i fältet **AffectedItems.**
    > [!NOTE]
    > Du kan inte återställa borttagna objekt med hjälp av granskningsloggfunktionen. Information om hur du återställer borttagna objekt [finns i Återskapa borttagna objekt eller e-post i Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)

Mer information finns i Söka [i Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)
