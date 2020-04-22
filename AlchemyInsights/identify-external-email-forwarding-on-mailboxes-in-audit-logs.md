---
title: Identifiera extern vidarebefordran av e-post på postlådor i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716478"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när extern vidarebefordran av e-post är konfigurerad på postlådor

När en Microsoft 365-användare konfigurerar extern vidarebefordran av e-post på en postlåda granskas aktiviteten som en del av cmdleten **Set-Mailbox.** Du kan se aktiviteten med hjälp av granskningsloggsökning i Security & Compliance Center.

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå till söksidan **för sökfunktionen i** > **sökgranskning.**

3. Välj datumintervall i fälten **Startdatum** och **Slutdatum.** Du behöver inte ange ett användarnamn. Kontrollera att fältet **Aktiviteter** är inställt på **Visa resultat för alla aktiviteter**.

4. Klicka på **Sök**.

I resultatet klickar du på **Filtrera resultat** och skriver **Set-Postlåda** i rutan aktivitetsfilter. Välj en granskningspost i resultatet. Klicka på **Mer information**i utfällbara **information.** Du måste titta på information om varje granskningspost för att avgöra om aktiviteten är relaterad till vidarebefordran av e-post.

- **ObjectId**: Aliasvärdet för postlådan som har ändrats.

- **Parametrar**: _ForwardingSmtpAddress_ anger målet e-postadress.

- **UserId**: Användaren som konfigurerade vidarebefordran av e-post på postlådan i fältet **ObjectId.**

Mer information finns i [Bestämma vem som konfigurerar vidarebefordran av e-post för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
