---
title: Synkronisering av Teams-kontakter
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: 0ffa91f0e31a4904db87f0df6d9b4c51b05ae2758a5ce0d96c77ef4456f6d033
ms.sourcegitcommit: 71501cde5bcb73f4dcf23944d400a4db10f37033
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/09/2021
ms.locfileid: "57807209"
---
# <a name="teams-contacts-sync"></a>Synkronisering av Teams-kontakter

Teams använder kontakter i organisationens Active Directory och kontakter som lagts till i användarens Outlook-standardmapp. Om kontakter inte visas i Microsoft Teams kan du prova följande:

**Obs!** Om informationen för en eller flera kontakter nyligen uppdaterades kan det ta upp till 48 timmar innan kontakterna synkroniseras.

1. Logga ut från Teams och starta om. Kontrollera om dina kontakter visas.
1. Rensa Teams-cachen:
    1. Bläddra till **%appdata%\Microsoft\Teams**.
    1. Ta bort innehållet i mappen.
    1. Starta om datorn och starta Teams.
1. Om kontakten finns i Outlook måste du lägga till den i kontaktlistan. I adressfältet i Outlook väljer du **Arkiv** och sedan **Lägg till kontakter**.
1. Kontrollera att användarens Exchange-postlåda finns online (inte lokalt). Mer information finns i [Så här interagerar Exchange och Microsoft Teams](/microsoftteams/exchange-teams-interact).
1. Kontrollera att kontaktens telefonnummer har lagts till i kontaktinformationen.
1. Sök efter kontaktens e-postadress i sökfältet. Kontakter som du kan hämta synkroniseras med kontaktlistan.
