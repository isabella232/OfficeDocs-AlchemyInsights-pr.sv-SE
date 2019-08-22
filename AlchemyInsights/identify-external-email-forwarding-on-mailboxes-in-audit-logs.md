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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539119"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när externa e-vidarebefordran har konfigurerats på postlådor

När en Office 365-användare konfigurerar externa e-vidarebefordring på en postlåda, granskade aktiviteten som en del av cmdlet **Set-postlåda** . Du kan se aktiviteten med Granska loggen Sök i säkerhet & regelefterlevnadscentret.

1. Logga in på [Office 365 säkerhet & regelefterlevnadscentret](https://protection.office.com/).

2. Gå till **Sök** > **Granska loggen** söksida.

3. Välj datumintervall i fälten **startdatum** och **slutdatum** . Du behöver inte ange ett användarnamn. Kontrollera fältet **verksamhet** är att **Visa resultat för alla aktiviteter**.

4. Klicka på **Sök**.

I resultaten klickar du på **Filtrera resultat** och skriv **Set-postlåda** i filterrutan aktivitet. Markera en granskningspost i resultaten. Klicka på **Mer information**i **information** -utfällbar. Du behöver titta på detaljerna i varje Granskningspost för att avgöra om aktiviteten är relaterad till e-post vidarebefordras.

- **Objekt-ID**: alias värdet för postlådan som ändrades.

- **Parametrar**: _ForwardingSmtpAddress_ anger den e-postadressen.

- **Användar-ID**: den användare som konfigurerats för vidarebefordring av e-post på postlådan i fältet **objekt-ID** .

Mer information finns i [fastställa som definierar e-vidarebefordran för en postlåda](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
