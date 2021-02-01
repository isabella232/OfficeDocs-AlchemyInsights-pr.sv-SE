---
title: Problem med autentiseringsuppgifter
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063720"
---
# <a name="issues-with-credentials"></a>Problem med autentiseringsuppgifter

Microsofts identitetsplattform och inloggningsflödet för [OAuth 2.0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver hur du programmerar direkt mot OAuth 2.0-klientautentiseringsflödet.

**Hur hanterar jag lösenord eller certifikatautentiseringsuppgifter för ett program?**

I Azure CLI kan du använda autentiseringsuppgifter för [az ad-app](https://docs.microsoft.com/cli/azure/ad/app/credential) till att ta bort, lista eller återställa ett programs lösenord eller certifikatuppgifter.

**Hur återställer mina användare sina lösenord?**

Användare måste [registrera sig för självbetjäning för återställning](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) av lösenord innan de kan återställa sina lösenord. När en användare har registrerat sig kan han eller hon följa anvisningarna i den här artikeln för att återställa lösenordet: Återställa lösenordet för [arbetet eller skolan.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hur ändrar mina användare sina lösenord?**

Användare kan följa stegen i den här artikeln för att ändra sina lösenord: [Så här ändrar du ditt lösenord.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De kan också [hantera applösenord för tvåstegsverifiering.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Användaren får ett felmeddelande när han eller hon ändrar eller återställer lösenordet**

Den här länken innehåller information om vanliga problem som kan uppstå när en användare försöker återställa sitt lösenord: [vanliga problem och deras lösningar](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jag har problem med att återställa en användares lösenord**

- Kontrollera att du har behörighet att återställa lösenord. *Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

- Se till att du förstår licenskraven:

  - Du måste ha minst en tilldelad licens i organisationen:
    - **Endast användare i molnet** – betald Office 365-SKU (O365) eller Azure AD Basic
    - **Molnanvändare och/eller** lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Mer information om licenskrav finns i [Licenskrav för självbetjäning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)för återställning av lösenord i Azure AD.
- Om du vill återställa en användares lösenord måste du hitta användaren i Azure AD. Klicka sedan på knappen "Återställ lösenord" i översiktsbladet för den användaren.

**Knappen för återställning av lösenord är nedtonad**

Du har inte behörighet att **återställa** den här användarens lösenord. *Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte bladet för återställning av lösenord**

Du har inte behörighet att återställa lösenord. *Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte det lokala integrationsbladet i lösenordsåterställning**

- Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lösenord för lokala användare.

- Du ser inte det här bladet om:

  - Du använder inte tillbakaskrivning av lösenord
  - Det är ett problem med återskrivning av lösenord vid installation/anslutning
  - Det är problem med installation/anslutning av Azure AD Connect
  - Mer felsökningssteg för problem med tillbakaskrivning av lösenord finns i Felsöka tillbakaskrivning [av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jag vet inte hur jag återställer en användares lösenord**

1. Logga in på Azure-portalen som lämplig administratör.
2. Gå till **bladet Användare och** grupper och välj Alla **användare.**
3. Välj en användare i listan.
4. Välj Översikt för **den** valda användaren och sedan Återställ lösenord i **kommandofältet.**
5. Välj knappen **Återställ lösenord** och följ instruktionerna på skärmen.
    - Återställningar utförs endast via **Azure Portal som har stöd** för återställning av lösenord.

**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilappen, men användaren kan fortfarande inte logga in**

Password Writeback stöds inte i den här portalen. Återställ användarens lösenord igen i Azure Portal.
