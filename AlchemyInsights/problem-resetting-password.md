---
title: Problem med återställning av lösenord
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039984"
---
# <a name="problems-resetting-password"></a>Problem med att återställa lösenord

Här är några av de problem som kan ha att göra med återställning av lösenord och möjliga lösningar:

**Jag har ett problem med återställning av lösenord som inte omfattas av andra kategorier**

- Se till att du har behörighet att återställa lösenord. Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.
- Se till att du förstår licenskraven:
    - Du måste ha minst en licens tilldelad i din organisation
        - Endast molnanvändare – alla Office 365 (O365) betal-SKU eller Azure AD Basic
        - Användare i molnet och/eller lokalt – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) Secure Productive Enterprise (SPE)
        - Mer information om licenskrav finns i artikeln [Licenskrav för självbetjäning för självbetjäning för Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag har problem med att testa principen för återställning av lösenord som jag anger**

- Nyligen använda principer kan ta flera minuter att replikera över alla datacenter och ändpunkter. Det fysiska avståndet från datacentret påverkar också hur snabbt ändringarna tillämpas.
- Testa med en slutanvändare, inte en administratör, och pilottesta med en liten uppsättning användare. Principerna som konfigurerats i Azure-portalen gäller ENDAST för slutanvändare, inte administratörer. Microsoft tillämpar en stark standardprincip med två grindar för återställning av lösenord för alla Azure-administratörsroller (exempel: global administratör, supportadministratör, lösenordsadministratör osv.)
    - Läs mer om [principer för administratörer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Jag vill distribuera återställning av lösenord men jag vill inte få mina användare att registrera ytterligare säkerhetsinformation**

Fyll i data för användarna i förväg så att de inte behöver det! – Som administratör kan du ange egenskaper för telefon och e-post för dina användare innan du distribuerar lösenordsåterställning till din organisation. Du kan göra detta med ett API, PowerShell eller Azure AD Anslut. Mer information finns här:
- [Distribuera lösenordsåterställning utan att användare måste registrera sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Vilka data används vid återställning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Knappen för återställning av lösenord är nedtonad**

Du har inte behörighet att återställa användarens lösenord. Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte bladet för återställning av lösenord**

Du har inte behörighet att återställa lösenord. Endast globala administratörer, lösenord och användaradministratörer kan återställa användarlösenord. Globala administratörer kan också återställa andra behöriga administratörers lösenord.

**Jag ser inte det lokala integrationsbladet i lösenordsåterställning**

- Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lokala användares lösenord.
- Det här bladet visas inte om:
    - Du använder inte tillbakaskrivning av lösenord
    - Det är problem med återskrivning av lösenord vid installation/anslutning
    - Det är problem med installation/anslutning av Azure AD-Anslut
    - Fler felsökningssteg för problem med tillbakaskrivning av lösenord finns i avsnittet Felsöka [tillbakaskrivning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jag vet inte hur jag återställer en användares lösenord**

1. Logga in på Azure Portal som lämplig administratör.
1. Gå till bladet Användare och grupper och välj **Alla användare.**
1. Välj en användare i listan.
1. För den valda användaren väljer du **Översikt** och klickar sedan på Återställ lösenord **i kommandofältet.**
1. Följ instruktionerna på skärmen.
    - Återställningar utförs endast via supportlösenord för Azure Portal.

**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilprogrammet, men användaren kan fortfarande inte logga in**

Password Writeback stöds inte i den här portalen. Återställ användarens lösenord igen i Azure Portal – portal.azure.com

