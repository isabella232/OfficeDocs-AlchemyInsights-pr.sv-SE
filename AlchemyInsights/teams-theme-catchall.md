---
title: Teams tema fånga allt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: 47e9aa76f8624ce3ddf4cfd03637b5b2714eb435
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030418"
---
# <a name="teams-common-issues-and-resolutions"></a>Vanliga problem och lösningar för Teams

**Viktigt**: På grund av den nyliga ökningen av Teams-användningen kan det ta cirka 24 timmar innan en användare är helt aktiverad efter det att du tilldelat en Teams-licens. Du kan inte tilldela Teams-principer till dem och de kanske inte har tillgång till vissa Teams-funktioner som samtal och ljudkonferenser förrän de aktiverats helt.

**Vanliga problem och lösningar**

Om du vill ha mer information kan du prova att formulera om frågan så att den innehåller fel som du kan se eller vilka Teams-funktioner du använder.

Om du behöver hjälp med att distribuera Teams för att stödja distansarbete(WFH) på grund av COVID-19 kan du granska [Stödja fjärrarbetarna med Microsoft Teams](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams). Du kan också vara berättigad till distributionsassistans från Microsoft 365 FastTrack-programmet. besök [Center för FastTrack](https://www.microsoft.com/fasttrack) för att skicka en begäran.

För alla teams kunder:

- **Ny till Teams?** Se [Komma igång med Microsoft Teams](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start).
- **Aktivera gäståtkomst i Teams:** Granska [Teams checklista för gäståtkomst](https://docs.microsoft.com/microsoftteams/guest-access-checklist) och se till att alla steg har slutförts. Fler resurser:
    - [Förstå gäståtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Konfiguration – checklista för gäståtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Hur gästen ansluter sig till ett team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams möten och inringningar**: Vill du ha hjälp med att aktivera eller konfigurera ljudkonferenser i Microsoft Teams? Har användaren skapats nyligen? I sådana fall måste du vänta 2-24 timmar **innan inställningarna börjar gälla**. 

    Kontrollera att användaren har en licens för ljudkonferenser och har ett avgiftsbelagt standardtelefonnummer:
    1.    Gå till Aktiva användare och markera den aktuella användaren.
    2.    Beroende på version av administratörscenter väljer du antingen **Licenser och appar** eller klickar **Redigera** på **Produktlicenser**.
    3.    Bekräfta att användaren har licenser valda för Ljudkonferens, Microsoft Teams och Skype för företag Online (abonnemang 2).
    4.    Användarens Administratörscenter, klicka på **Visa alla** och sedan **Teams**.
    5.    I administrationscentret för Microsoft Teams klickar du på **Äldre portal**.
    6.    I administrationscentret för Skype för företag klickar du på **Ljudkonferens** och sedan **Användare**.
    7.    Välj användaren i fråga och kontrollera att användaren har ett Avgiftsbelagt standardnummer.
    
    För mer information i [Samtalsabonnemang för Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) eller ring Microsoft Commerce Billing-teamet för att få hjälp med licensrelaterade frågor.

    Ytterligare resurser:

    - [Möten och konferenser i Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Ljudkonferens i Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Teams Exploratory-licens**: Microsofts Teams Exploratory upplevelse tillåter användare i organisationen som har Azure Active Directory (AAD) och som inte har licens för Teams kan starta en exploratory-upplevelse av Teams. Administratörer kan aktivera eller inaktivera den här funktionen för användare i organisationen. Den tidigare [utvärderingsversionen av Microsofts kommersiella moln](https://docs.microsoft.com/microsoftteams/iw-trial-teams) har nu ersatts av exploratory-upplevelse av Teams.

    Ytterligare resurser:

    - [Hur användare registrerar sig för exploratory-upplevelse i Teams](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience)
    - [Hantera exploratory-upplevelsen för Teams](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience)

- **Privata kanaler**: privata kanaler i Microsoft Teams skapar fokuserade utrymmen för samarbete i dina grupper. Det är bara användare i teamet som är ägare eller medlemmar i den privata kanalen som kan komma åt kanalen. Alla, inklusive gäster, kan läggas till som medlemmar i en privat kanal så länge de är medlemmar i gruppen.

    Du kanske vill använda en privat kanal om du vill begränsa samarbetet till dem som har ett behov av att veta eller om du vill under lätta kommunikationen mellan en grupp personer som är kopplade till ett särskilt projekt, utan att behöva skapa ytterligare ett team att hantera.

    Ytterligare resurser:
    - [Skapande och medlemskap för privat kanal](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership)
    - [Hantera medlemskap och inställningar i en privat kanal](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings)

- **Mötesprinciper**: Mötesprinciper används för att kontrollera vilka funktioner som är tillgängliga för mötesdeltagare i möten som är schemalagda av användare i organisationen. När du har skapat en princip och gjort dina ändringar kan du tilldela användare till principen. 
    - **Ändra eller skapa en mötespolicy**: du kan ändra eller skapa en mötespolicy genom att gå till **Microsoft Teams administrationscenter > Möten > Mötesprinciper**. Välj en princip från listan eller välj Lägg till. Om du skapar en ny princip kan du lägga till ett namn och en beskrivning. Namnet får inte innehålla specialtecken eller vara längre än 64 tecken. Välj önskade inställningar och klicka på **OK**.

        Anta till exempel att du har ett stort antal användare och vill begränsa mängden bandbredd som deras möten skulle behöva. Du kan skapa en ny anpassad princip med namnet "Begränsad bandbredd" och inaktivera följande inställningar:

        Under **Ljud och video**:
        - Inaktivera Tillåt molninspelning.
        - Inaktivera Tillåt IP-video.

        Under **Innehållsdelning**:
        - Inaktivera skärmdelningsläge.
        - Inaktivera Tillåt whiteboard.
        - Inaktivera Tillåt delade anteckningar.

        Tilldela sedan principen till användarna.

- **Tilldela en mötespolicy till användare**

    1. I den vänstra navigeringen i administrationscentret för Microsoft Teams går du till **Användare**och klicka sedan på användaren.
    2. Markera användaren genom att klicka till vänster om användarnamnet och sedan klicka på **Redigera inställningar**.
    3. Under **Mötesprincip** väljer du den princip du vill till dela och klickar sedan på **Använd**.

    Information om hur du tilldelar en princip till flera användare i taget finns i [Redigera användarinställningar i bulk för Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk). Du kan göra följande:

    1. I vänstra navigeringen i administrationscentret för Microsoft Teams och gå till **Möten > Mötesprinciper**.
    2. Välj principen genom att klicka till vänster om policynamnet.
    3. Välj **Hantera användare**.
    4. I fönstret **Hantera användare** kan du söka efter användar efter visningsnamn eller efter användarnamn, välja namnet och sedan klicka på **Lägg till**. Upprepa detta steg för alla användare du vill lägga till.
    5. När du är klar med att lägga till användare klickar du på **Spara**.

- **Felsöka en knappsats som saknas:**  

    - Kontrollera att användaren har tilldelats en [Teams-licens](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Kontrollera att användaren har en [Samtalsplan](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) tilldelad.
    - Aktivera användarna för [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Felsöka inloggning i Teams:** Börja med att kontrollera att [Microsoft Teams-tjänsten är frisk](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Leta sedan efter vanliga felkoder och granska [Varför kan jag ha problem med att logga in på Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)  Du kan också behöva granska [identitetsmodeller och autentisering i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

**För utbildningskunder:**

Om användarna ser meddelandet "Du missar detta!" Se till att du [Aktiverar Microsoft Teams för skolan](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). I EDU-klientorganisationer är Microsoft Teams inte aktiverat som standard. Du måste aktivera den först.

Granska [Utbildning och inlärning på distans i Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) för den senaste anvisningarna för att konfigurera skolan, lektionsplanering, virtuella möten och dela innehåll med elever.

Slutligen är det viktigt att ta en titt på träningsvideor, -kortlekar och mycket mer för Microsoft Teams IT-admin här: https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training. 
