---
title: Problem med att återställa lösenord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696279"
---
# <a name="problems-resetting-password"></a>Problem med att återställa lösenord

Här är några av de problem som kan finnas när du återställer lösenordet och möjliga lösningar:

**Jag har ett problem med återställning av lösenord som inte omfattas av de andra kategorierna**

- Se till att du har behörighet att återställa lösenord. Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.
- Se till att du förstår licenskraven:
    - Du måste ha minst en tilldelad licens i organisationen
        - Endast användare i molnet – betald Office 365-SKU (O365) eller Azure AD Basic
        - Molnanvändare och/eller lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
        - Mer information om licenskrav finns i artikeln [Licenskrav för självbetjäning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)för återställning av lösenord i Azure AD.

**Jag har problem med att testa principen för återställning av lösenord som jag har angett**

- Nyligen använda principer kan ta flera minuter att replikera över alla datacenter och ändpunkter. Det fysiska avståndet från datacentret påverkar också hur snabbt ändringar tillämpas.
- Testa med en slutanvändare, inte en administratör, och pilottesta med en liten uppsättning användare. Principerna som konfigurerats i Azure-portalen gäller ENDAST för slutanvändare, inte administratörer. Microsoft tillämpar en stark standardprincip med tvådelar för återställning av lösenord för alla Azure-administratörsroller (exempel: global administratör, supportadministratör, lösenordsadministratör osv.)
    - Läs mer om [principer för administratörer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Jag vill distribuera återställning av lösenord men jag vill inte göra så att användarna registrerar ytterligare säkerhetsinformation**

Fyll i data för användarna i förväg så att de inte behöver det! – Som administratör kan du ange telefon- och e-postegenskaper för användarna innan du distribuerar lösenordsåterställning till din organisation. Du kan göra detta med ett API, PowerShell eller Azure AD Connect. Mer information finns här:
- [Distribuera lösenordsåterställning utan att användare måste registrera sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Vilka data används vid återställning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Knappen för återställning av lösenord är nedtonad**

Du har inte behörighet att återställa den här användarens lösenord. Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte bladet för återställning av lösenord**

Du har inte behörighet att återställa lösenord. Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte bladet för lokal integrering i lösenordsåterställning**

- Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lösenord för lokala användare.
- Du ser inte det här bladet om:
    - Du använder inte tillbakaskrivning av lösenord
    - Det är ett problem med återskrivning av lösenord vid installation/anslutning
    - Det är problem med installation/anslutning av Azure AD Connect
    - Fler felsökningssteg för problem med tillbakaskrivning av lösenord finns i avsnittet [Felsöka tillbakaskrivning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag vet inte hur jag återställer en användares lösenord**

1. Logga in på Azure-portalen som lämplig administratör.
1. Gå till bladet Användare och grupper och välj **Alla användare.**
1. Välj en användare i listan.
1. Välj Översikt för den valda användaren **och** klicka sedan på Återställ lösenord i **kommandofältet.**
1. Följ instruktionerna på skärmen.
    - Återställningar utförs endast via Azure Portal som har stöd för återställning av lösenord.

**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilappen, men användaren kan fortfarande inte logga in**

Password Writeback stöds inte i den här portalen. Återställ användarens lösenord igen i Azure Portal – portal.azure.com

