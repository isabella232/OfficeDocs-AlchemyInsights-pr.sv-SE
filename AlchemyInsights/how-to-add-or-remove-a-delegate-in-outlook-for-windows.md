---
title: Lägga till eller ta bort ett ombud i Outlook för Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329058"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Lägga till eller ta bort ett ombud i Outlook för Windows

Så här lägger du till ett ombud i Outlook för Windows: 

1. Klicka på fliken **Arkiv** följt av **Konto Inställningar** och välj sedan **Ombud.**
2. Klicka på Lägg **till**. Om **Lägg** till inte visas kanske det inte finns någon aktiv anslutning mellan Outlook och Exchange. Statusfältet Outlook visar anslutningsstatus.
3. Skriv namnet på den person som du vill utse till ombud eller sök och välj namnet i listan med sökresultat.

    **Obs!** Ombudet måste vara en person i organisationens Exchange globala adresslistan (GAL).
4. Klicka på **Lägg till** följt av **OK.**
5. I dialogrutan **Behörigheter för** ombud accepterar du standardbehörighetsinställningarna eller väljer anpassade åtkomstnivåer för Exchange mappar.

    - Om ett ombud endast behöver behörighet för mötesförfrågningar och svar på mötesförfrågningar, är standardinställningarna, till exempel Ombudet får kopior på de **mötesrelaterade** meddelanden som skickats till mig tillräckliga. Du kan lämna **behörighetsinställningen** för Inkorgen hos **Ingen.** Mötesförfrågningar och svar på mötesförfrågningar skickas direkt till ombudens inkorg.

    **Obs!** Som standard får ombudet **behörigheten Redaktör (kan läsa, skapa och ändra objekt)** för **mappen** Kalender. När ombudet svarar på ett möte för din räkning läggs det automatiskt till i **mappen** Kalender.

5. Om du vill skicka ett meddelande med information om de ändrade behörigheterna till ombudet markerar du kryssrutan Skicka automatiskt ett meddelande till ombudet med en sammanfattning **av** behörigheterna.
6. Om du vill markerar du **kryssrutan Ombud kan se mina privata** objekt.

    **Viktigt:** Den här inställningen påverkar alla Exchange mappar. Det omfattar alla mapparna E-post, Kontakter, Kalender, Uppgifter, Anteckningar och Journal. Det går inte att ge åtkomst till privata objekt i endast angivna mappar.

7. Välj **OK**.

    **Obs!**
    - I meddelanden som skickas med behörigheten Skicka för visas både ombudens och ditt namn bredvid **Från**. När ett meddelande skickas med behörigheten Skicka som visas bara ditt namn.
    - När du har lagt till någon som ombud kan de lägga till Exchange postlåda i sin Outlook postlåda. Anvisningar finns i Hantera [andra personers e-post- och kalenderobjekt.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)

Så här tar du bort ett ombud i Outlook för Windows:

1. Klicka på **fliken** Arkiv.
2. Klicka på **Konto Inställningar** följt av **Ombud**.
3. Välj namnet på det ombud som du vill ändra behörigheter för och klicka sedan på Ta **bort** följt av **OK.**
