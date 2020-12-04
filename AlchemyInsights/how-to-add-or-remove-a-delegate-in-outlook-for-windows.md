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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573811"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Lägga till eller ta bort ett ombud i Outlook för Windows

Så här lägger du till ett ombud i Outlook för Windows: 

1. Klicka på fliken **Arkiv** följt av **konto inställningar** och välj sedan **ombud**.
2. Klicka på **Lägg till**. Om **Lägg till** inte visas kan det bero på att det inte finns en aktiv anslutning mellan Outlook och Exchange. I statusfältet i Outlook visas anslutnings status.
3. Skriv namnet på den person du vill ange som ombud, eller Sök och välj namnet i listan Sök resultat.

    > [!NOTE]
    > Ombudet måste vara en person i organisationens globala adress lista (GAL).
4. Klicka på **Lägg till** följt av **OK**.
5. Godkänn standardinställningarna i dialog rutan **behörigheter för ombud** eller Välj anpassade åtkomst nivåer för Exchange-mappar.

    - Om ett ombud behöver behörighet att endast arbeta med Mötes förfrågningar och svar är det tillräckligt med de förvalda behörighets inställningarna, till exempel **ombud** . Du kan lämna behörighets inställningen för **Inkorgen** **.** Mötes förfrågningar och svar skickas direkt till ombudets inkorg.

    > [!NOTE]
    > Som standard tillåts ombudet **(kan läsa, skapa och ändra objekt)** behörighet till mappen **kalender** . När ombudet svarar på ett möte åt dig läggs det automatiskt till i mappen **kalender** .

5. Om du vill skicka ett meddelande om du vill meddela ombudet om de ändrade behörigheterna markerar du kryss rutan **Skicka automatiskt ett meddelande till ombudet om att sammanfatta dessa behörigheter** .
6. Markera kryss rutan **ombud kan se mina privata objekt** om du vill.

    > [!IMPORTANT]
    > Den här inställningen påverkar alla Exchange-mappar. Detta inkluderar all e-post, kontakter, kalender, uppgifter, anteckningar och journalmallar. Det finns inget sätt att bevilja åtkomst till privata objekt i endast angivna mappar.

7. Välj **OK**.

    > [!NOTE]
    >
    > - Meddelanden som skickas med behörigheter för skicka i uppdrag inkluderar både ombudets och deras namn bredvid **från**. När ett meddelande skickas med skicka som-behörighet visas bara ditt namn.
    > - När du lägger till någon som ombud kan de lägga till din Exchange-postlåda i sin Outlook-profil. Anvisningar finns i [hantera en annan persons e-post och Kalender objekt](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Så här tar du bort ett ombud i Outlook för Windows:

1. Klicka på fliken **Arkiv** .
2. Klicka på **konto inställningar** följt av **ombuds åtkomst**.
3. Välj namnet på det ombud som du vill ändra behörigheter för och klicka sedan på **ta bort** följt av **OK**.
