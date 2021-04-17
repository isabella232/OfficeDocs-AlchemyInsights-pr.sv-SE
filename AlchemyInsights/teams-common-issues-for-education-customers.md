---
title: Vanliga Teams-problem för utbildningskunder
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
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 6d1fac07673f6f945f382e4e640cf44afb76717d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829466"
---
# <a name="teams-common-issues-for-education-customers"></a>Vanliga Teams-problem för utbildningskunder

**För utbildningskunder**:

Om du behöver hjälp med att distribuera Teams för att få support via fjärrhjälp går du till [FastTrack Center](https://www.microsoft.com/fasttrack) för att skicka en begäran. Se följande vanliga problem för Teams utbildningskunder:

- Ser du meddelandet "**Du missar detta!**"? Se till att du [Aktiverar Microsoft Teams för skolan](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). I EDU-klientorganisationer är Microsoft Teams inte aktiverat som standard. Du måste aktivera den först.

- **Ny på Teams?** Läs [Utbildning och inlärning på distans i Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) för de senaste anvisningarna för att konfigurera skolan, lektionsplanering, virtuella möten och dela innehåll med elever.

- När det aktiverats kan användarna köra Teams, antingen genom att installera [skrivbordsversionen](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) eller [mobila klienter,](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) eller i webbläsaren på https://teams.microsoft.com.

- **Aktivera gäståtkomst i Teams**: Granska [Teams checklista för gäståtkomst](https://docs.microsoft.com/microsoftteams/guest-access-checklist) och se till att alla steg har slutförts.
    - [Förstå gäståtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Konfiguration – checklista för gäståtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Hur gästen ansluter sig till ett team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams möten och inringningar**: Vill du ha hjälp med att aktivera eller konfigurera ljudkonferenser i Microsoft Teams? Har användaren skapats nyligen? I sådana fall måste du vänta 2-24 timmar innan inställningarna börjar gälla. Kontrollera att användaren har en licens för ljudkonferenser och har ett avgiftsbelagt standardtelefonnummer:
    1. Gå till Aktiva användare och markera den aktuella användaren.
    2. Beroende på version av administratörscenter väljer du antingen **Licenser och appar** eller klickar **Redigera** på **Produktlicenser**.
    3. Bekräfta att användaren har licenser valda för Ljudkonferens, Microsoft Teams och Skype för företag Online (abonnemang 2).
    4. Användarens Administratörscenter, klicka på **Visa alla** och sedan **Teams**.
    5. I administrationscentret för Microsoft Teams klickar du på **Äldre portal**.
    6. I administrationscentret för Skype för företag klickar du på **Ljudkonferens** och sedan **Användare**.
    7. Välj användaren i fråga och kontrollera att användaren har ett Avgiftsbelagt standardnummer.

    Mer information finns i [Planer för att ringa med Microsoft Teams](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365), eller ring Microsoft Commerce Billing-teamet för att få hjälp med licensrelaterade frågor.

    Ytterligare resurser

    - [Möten och konferenser i Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Ljudkonferens](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Mötesprinciper**: Mötesprinciper används för att kontrollera de funktioner som är tillgängliga för mötesdeltagare i möten schemalagda av användare i organisationen. Efter att du skapat en princip och gjort dina ändringar kan du tilldela användare till principen.

    - **Ändra eller skapa en mötespolicy**: du kan ändra eller skapa en mötespolicy genom att gå till **Microsoft Teams administrationscenter > Möten > Mötesprinciper**. Välj en princip från listan eller klicka på **Lägg till**. Om du skapar en ny princip kan du lägga till ett namn och en beskrivning. Namnet får inte innehålla specialtecken eller vara längre än 64 tecken. Välj önskade inställningar och klicka på **OK**. 
    
        Anta till exempel att du har ett stort antal användare och vill begränsa bandbredden som deras möten skulle behöva. Du kan skapa en ny anpassad princip med namnet "Begränsad bandbredd" och inaktivera följande inställningar:

        Under **Ljud och video**:
        - Inaktivera **Tillåt molninspelning**.
        - Inaktivera **Tillåt IP-video**.

        Under **Innehållsdelning**:

        - Inaktivera skärmdelningsläge.
        - Inaktivera **Tillåt whiteboard**.
        - Inaktivera **Tillåt delade anteckningar**.

        Tilldela **sedan principen till användarna**:

    1. I den vänstra navigeringen i administrationscentret för Microsoft Teams går du till **Användare**, klicka sedan på användaren.
    2. Markera användaren genom att klicka till vänster om användarnamnet och sedan klicka på **Redigera inställningar**.
    3. Under **Mötesprincip** väljer du den princip du vill till dela och klickar på **Använd**.

    Information om hur du tilldelar en princip till flera användare i taget finns i [Redigera användarinställningar i bulk för Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Du kan göra följande:
    1. I vänstra navigeringen i administrationscentret för Microsoft Teams och gå till **Möten > Mötesprinciper**.
    2. Välj principen genom att klicka till vänster om policynamnet.
    3. Klicka på **Hantera användare**.
    4. I fönstret **Hantera användare** kan du söka efter användar efter visningsnamn eller efter användarnamn, välja namnet och sedan klicka på **Lägg till**. Upprepa detta steg för alla användare du vill lägga till.
    5. När du är klar med att lägga till användare klickar du på **Spara**.

- **Felsöka en knappsats som saknas**:
    - Kontrollera att användaren har tilldelats en [Teams-licens](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Kontrollera att användaren har en [Samtalsplan](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) tilldelad.
    - Aktivera användarna för [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Felsöka inloggning i Teams**: Börja med att kontrollera att [Microsoft Teams-tjänsten är frisk](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Leta sedan efter vanliga felkoder och granska [Varför kan jag ha problem med att logga in på Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)? Du kan också behöva granska [identitetsmodeller och autentisering i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
