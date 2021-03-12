---
title: Felsöka gruppproblem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714446"
---
# <a name="troubleshoot-group-issues"></a>Felsöka gruppproblem

**Jag behöver tilldela en grupp till en Azure AD-roll**

Så här tilldelar du en Azure Active Directory-grupp (AD) till en Azure AD-roll:

1. Skapa en ny grupp – så här skapar du en ny grupp:

    a. Logga in på administrationscentret för Azure AD med behörighet som rolladministratör eller global administratörsbehörighet. 
    b. Välj Azure Active Directory > grupper > alla grupper > Ny grupp. 
    c. Skapa gruppen.

2. Tilldela rollen till gruppen antingen när gruppen skapas eller när den har skapats.

    a. Om du vill tilldela en roll till gruppen när gruppen skapas, aktiverar du växlingsknappen för Azure AD-roller och kan tilldelas gruppen och skapa gruppen.
    b. Om du vill tilldela en roll till gruppen efter att den har skapats går du till fliken Tilldelade roller för den nya gruppen och tilldelar rollen till gruppen.

**Jag behöver hantera medlemskap i en grupp som har tilldelats rollen Azure AD**

1. För att förhindra ökning av behörigheter kan som standard endast administratör för privilegierad roll och global administratör ändra medlemskapet för en grupp som har tilldelats till en roll. De kan däremot välja att tilldela en ägare för en sådan grupp och delegera den här uppgiften. Mer information finns i Använda [molngrupper för att hantera rolltilldelningar i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. För vanliga frågor och felsökningstips för att tilldela roller till grupper i Azure AD, se [Felsökningsroller som tilldelats molngrupper.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dynamiska grupper**

1. Om du inte hittar de inbyggda användarattributen, kontrollera att attributet finns i listan med egenskaper som stöds.
2. Om du letar efter inbyggda enhetsattribut ser du till att attributet finns i listan med enhetsattribut 
3. Förutom de inbyggda användar- och enhetsattributen kan du också använda [tilläggsattribut.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) När du har synkroniserat tilläggsattribut från en lokal Windows Server AD eller från ett anslutet SaaS-program ska attributen vara synliga i listrutan i regelverktyget. Du hittar det anpassade attributnamnet i katalogen genom att fråga en användares attribut med Hjälp av PowerShell och söka efter attributnamnet. De kan också användas när du skapar regler i regelsyntaxen.
4. Kontrollera att klientorganisationen har rätt licens. Dynamiska grupper kräver att klientorganisationen har en Licens för Azure AD P1 Premium. Listan med Azure AD-licensplaner finns [här.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security-licensplaner kan nås [här.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Se till att rollen för användaren som skapar den dynamiska gruppen är en global administratör, intune-administratör, gruppadministratör eller en användaradministratör.
6. Ange att gruppen ska fyllas i. Beroende på klientorganisationens storlek kan gruppen ta upp till 24 timmar för att fyllas i för första gången eller efter en regeländring.
7. Mer information finns i Skapa [attributbaserade regler för dynamiskt gruppmedlemskap.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Jag behöver ta bort en grupp**

1. Grupper kan tas bort från katalogen med hjälp Remove-AzureADGroup cmdlet i Azure AD Powershell-modulen.
2. Innan du försöker ta bort en synkroniserad grupp i Azure AD bör du kontrollera att du har tagit bort alla tilldelade licenser för att undvika fel.
3. Mer information om hur du tar bort grupper finns [i Ta bort en grupp med en tilldelad licens.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Jag behöver återställa en borttagna grupp**

1. Om en Office 365-grupp tas bort kan den bara återställas upp till 30 dagar innan permanent borttagning sker. När gruppen har tagits bort permanent går det inte längre att återställa den. Läs mer om att återställa grupper [här.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Den här funktionen stöds inte för säkerhetsgrupper och distributionsgrupper.
3. Kontrollera att du har behörighet att återställa en Office 365-grupp. Globala administratörer, gruppadministratörer, användarkontoadministratörer, intune-tjänstadministratörer, support på partnernivå eller nivå2 och gruppens ägare kan återställa en grupp.
4. När en dynamisk grupp tas bort och återställs, ses den som en ny grupp och fylls i på nytt enligt regeln. Den här processen kan ta upp till 24 timmar.
5. Mer information om hur du återställer en borttagna grupp finns i [Återställa en borttagna Office 365-grupp i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Konfiguration av förfalloprincip för grupp**

1. Den här funktionen stöds endast för Office 365-grupper och inte för säkerhetsgrupper och distributionsgrupper.
2. För att konfigurera och använda förfalloprincipen för Office 365-grupper krävs en Azure AD Premium-licens.
3. För närvarande kan endast en förfalloprincip konfigureras för Office 365-grupper i en innehavare.
4. Endast globala administratörer, gruppadministratörer, användaradministratörer och gruppens ägare kan förnya en grupp.
5. Om en Office 365-grupp upphör att gälla tas den bort och kan bara återställas upp till 30 dagar innan permanent borttagning sker. När gruppen har tagits bort permanent går det inte längre att återställa den. Läs mer om att återställa grupper [här.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Aktivitetsbaserad automatisk förnyelse**

Användaraktiviteter från SharePoint, Outlook och Teams kan utlösa automatisk gruppförnyelse. Aktiviteter kontrolleras 35 dagar innan en grupp går ut. Om det finns aktivitet under den aktuella grupplivscykeln förnyas gruppen automatiskt och e-postaviseringar skickas inte ut till gruppens ägare.

**Tidsinställningar för meddelanden för in utgångna grupper**

1. E-postmeddelanden skickas till Office 365-gruppägarna 30 dagar, 15 dagar och 1 dag innan gruppen upphör.
2. När du först ställer in förfallotid sätts alla grupper som är äldre än utgångsintervallet till 35 dagar till förfallodatumet.
3. Gruppens förfallodatum beräknas baserat på gruppens förnyelsedatum, inte baserat på datumet då principen uppdaterades. Om förfalloprincipen uppdateras ändras inte utgångsdatumet.
4. Mer information finns i [e-postmeddelanden om förfalloprinciper](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) för grupper och förnyelse av e-postmeddelanden och Återställa en [borttagna Office 365-grupp i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Behörighet att skapa en grupp**

Kontrollera att du har behörighet att skapa en ny grupp. Globala administratörer kan inaktivera skapande av grupper i Azure-portalen eller Åtkomstpanelen. Du kan behöva en administratör för att skapa den nya gruppen åt dig eller ge dig rätt behörigheter.

1. [Skapa en ny grupp och lägga till medlemmar i Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Skapa grupper i Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Inaktivera skapande av grupper i Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Hantera vem som kan skapa grupper i Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Inaktivera välkomstmeddelande i Office 365 via Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD-administratörsroller](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Hantera behörigheter för att skapa grupper**

1. Globala administratörer kan hantera behörigheter för skapande av grupper för säkerhet eller Office 365-grupper som skapats i Azure-portalen eller åtkomstpanelen genom att ange att användare kan skapa säkerhetsgrupper i **Azure-portaler** eller användare kan skapa **Office 365-grupper** i Azure Portals-inställningar i Alla grupper **> Allmänt (Inställningar).**
2. Du kan också begränsa skapandet av grupper för att välja en grupp användare om du har en Azure AD P1 Premium-licens.

**Inaktivera välkomstmeddelande för nya medlemmar i en Office 365-grupp**

Välkomstmeddelandet som skickas till användare som har lagts till i Office 365-grupper kan inaktiveras genom att ange `UnifiedGroupWelcomeMessageEnabled` **inställningen False** i Powershell. Läs mer om den [här](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)inställningen.













