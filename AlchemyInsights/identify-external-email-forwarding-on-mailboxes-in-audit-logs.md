---
title: Identifiera externa e-vidarebefordran på postlådor i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383115"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när externa e-vidarebefordran har konfigurerats på postlådor

När en användare konfigurerar externa e-vidarebefordring på en postlåda, granskade aktiviteten som en del av cmdlet **Set-postlåda** . Du kan se aktiviteten med Granska loggen Sök i säkerhet & regelefterlevnadscentret.

1. Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)

2. Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.

3. Välj datumintervall i fälten **startdatum** och **slutdatum** . Du behöver inte ange ett användarnamn. Kontrollera fältet **verksamhet** är att **Visa resultat för alla aktiviteter**.

4. Klicka på **Sök**.

I resultaten klickar du på **Filtrera resultat** och skriv **Set-postlåda** i filterrutan aktivitet. Markera en granskningspost i resultaten. Klicka på **Mer information**i **information** -utfällbar. Du behöver titta på detaljerna i varje Granskningspost för att avgöra om aktiviteten är relaterad till e-post vidarebefordras.

- **Objekt-ID**: alias värdet för postlådan som ändrades.

- **Parametrar**: _ForwardingSmtpAddress_ anger den e-postadressen.

- **Användar-ID**: den användare som konfigurerats för vidarebefordring av e-post på postlådan i fältet **objekt-ID** .

Mer information finns i [fastställa som definierar e-vidarebefordran för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
