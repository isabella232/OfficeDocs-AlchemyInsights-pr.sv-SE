---
title: Identifiera extern vidarebefordran av e-post i postlådor i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028773"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när extern vidarebefordran av e-post konfigureras för postlådor

När en Microsoft 365 konfigurerar extern vidarebefordran av e-post för en postlåda granskas aktiviteten som en del av cmdleten **Set-Mailbox.** Du kan se aktiviteten med hjälp av granskningsloggsökning i Säkerhets- & efterlevnadscenter.

1. Logga in på [Microsoft 365 Kompatibilitetscenter.](https://protection.office.com/)

2. Gå till sidan **Sök**  >  **granskningsloggsökning.**

3. Välj datumintervallet i **fälten Startdatum** **och** Slutdatum. Du behöver inte ange ett användarnamn. Kontrollera att **fältet** Aktiviteter är inställt **på Visa resultat för alla aktiviteter.**

4. Klicka **på Sök**.

I resultatet klickar du på **Filtrera resultat** och **skriver Set-Mailbox** i aktivitetsfilterrutan. Välj en granskningspost i resultatet. Klicka på **Mer** information i den **utfällna menyn Information.** Du måste granska informationen för varje granskningspost för att avgöra om aktiviteten är relaterad till vidarebefordran av e-post.

- **ObjectId:** Aliasvärdet för postlådan som ändrades.

- **Parametrar:** _ForwardingSmtpAddress_ anger målets e-postadress.

- **UserId:** Användaren som konfigurerade vidarebefordran av e-post för postlådan i **fältet ObjectId.**

Mer information finns i Fastställa [vem som har konfigurerat vidarebefordran av e-post för en postlåda.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
