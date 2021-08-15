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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986837"
---
# <a name="issues-with-credentials"></a>Problem med autentiseringsuppgifter

Microsofts identitetsplattform och [OAuth 2.0-klientautentiseringsflödet](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver hur du programar direkt mot OAuth 2.0-klientautentiseringsflödet.

**Hur hanterar jag lösenord eller certifikatautentiseringsuppgifter för ett program?**

I Azure CLI kan du använda [autentiseringsuppgifter](https://docs.microsoft.com/cli/azure/ad/app/credential) för az ad-appen till att ta bort, lista eller återställa lösenord eller certifikatautentiseringsuppgifter för ett program.

**Hur återställer mina användare sina lösenord?**

Användarna måste [registrera sig för återställning av lösenord innan](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) de kan återställa sina lösenord. När en användare har registrerat sig kan de följa instruktionerna i den här artikeln för att återställa sitt lösenord: Återställa ditt [arbets- eller skollösenord](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Hur ändrar mina användare sina lösenord?**

Användare kan ändra sina lösenord genom att följa stegen i den här artikeln: [Så här ändrar du ditt lösenord.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De kan också [Hantera applösenord för tvåstegsverifiering.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Användaren får ett felmeddelande när han eller hon ändrar eller återställer lösenordet**

Den här länken ger information om vanliga problem som kan uppstå när en användare försöker återställa sitt lösenord: [vanliga problem och deras lösningar](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jag har problem med att återställa en användares lösenord**

- Se till att du har behörighet att återställa lösenord. *Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

- Se till att du förstår licenskraven:

  - Du måste ha minst en licens tilldelad i din organisation:
    - **Endast molnanvändare** – alla Office 365 (O365) betal-SKU eller Azure AD Basic
    - **Användare i molnet och/eller** lokalt – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Mer information om licenskrav finns i Licenskrav för självbetjäning för [självbetjäning för Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Om du vill återställa en användares lösenord måste du hitta användaren i Azure AD. Klicka sedan på knappen "återställ lösenord" i översiktsbladet för den användaren.

**Knappen för återställning av lösenord är nedtonad**

Du har inte behörighet att **återställa** användarens lösenord. *Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte bladet för återställning av lösenord**

Du har inte behörighet att återställa lösenord. *Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord.* Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte det lokala integrationsbladet i lösenordsåterställning**

- Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lokala användares lösenord.

- Det här bladet visas inte om:

  - Du använder inte tillbakaskrivning av lösenord
  - Det är problem med återskrivning av lösenord vid installation/anslutning
  - Det är problem med installation/anslutning av Azure AD-Anslut
  - Mer information om felsökning av problem med tillbakaskrivning av lösenord finns i [Felsöka tillbakaskrivning av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jag vet inte hur jag återställer en användares lösenord**

1. Logga in på Azure Portal som lämplig administratör.
2. Gå till **bladet Användare och** grupper och välj Alla **användare.**
3. Välj en användare i listan.
4. För den valda användaren väljer **du Översikt** och sedan Återställ lösenord i **kommandofältet.**
5. Välj **knappen Återställ** lösenord och följ instruktionerna på skärmen.
    - Återställningar utförs endast via **supportlösenord för Azure Portal.**

**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilprogrammet, men användaren kan fortfarande inte logga in**

Password Writeback stöds inte i den här portalen. Återställ användarens lösenord igen i Azure Portal.
