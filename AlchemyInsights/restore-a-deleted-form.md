---
title: Återställa ett borttagna formulär
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809493"
---
# <a name="restore-a-deleted-form"></a>Återställa ett borttagna formulär

Om du har tagit bort ett formulär i Microsoft Forms av misstag kan du återställa det. Logga in på Microsoft Forms som ägare av det borttagna formuläret. Välj **Papperskorgen och välj** sedan det formulär du vill återställa och välj **Återställ.** När återställningen är återställd väljer **du sidpilen Tillbaka till sidan** Formulär.

Endast ägaren av formuläret kan återställa det. Om formulärägarens konto har inaktiverats eller tagits bort från klientorganisationen kan bara den globala administratören återställa formuläret. Den globala administratören måste ha en Forms-licens för att kunna återställa. Endast formulär som skapats inom 30 dagar efter att användarkontot inaktiverats eller tagits bort från klientorganisationen kan återställas.

Om du är global administratör för klientorganisationen och du vill återställa ett formulär från ett konto som har tagits bort eller inaktiverats ersätter du [e-postadress] med e-postadressen för den borttagna eller inaktiverade användaren i följande URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner= [e-postadress]** Om din e-postadress till exempel är johndoe@contoso.com, skulle URL:en vara: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** . 

När du har åtkomst till användarens borttagna formulär markerar du det formulär som du vill flytta och väljer sedan **Fler formuläråtgärder**  >  **Flytta.**

Om du vill återställa ett formulär där det togs bort och användaren togs bort från organisationen kan en global administratör välja att återställa användaren, återställa lösenordet för användaren och sedan logga in som användare för att flytta det till en annan aktiv användare. 