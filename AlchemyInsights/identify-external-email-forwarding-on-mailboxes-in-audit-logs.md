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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331177"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifiera när extern vidarebefordran av e-post konfigureras för postlådor

När en Microsoft 365 konfigurerar extern vidarebefordran av e-post för en postlåda granskas aktiviteten som en del av cmdleten **Set-Mailbox.** Du kan se aktiviteten med hjälp av granskningsloggsökning. Så här gör du.

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://sip.security.microsoft.com/auditlogsearch> Granskning.

2. På sidan **Granska** kontrollerar du att **fliken Sök** är markerad och konfigurerar sedan följande inställningar:
   - Välj datum-/tidsintervallet i **rutorna Start** **och** Slut.
   - Kontrollera att **rutan** Aktiviteter innehåller **Visa resultat för alla aktiviteter.**

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. I resultatet klickar du på **Filtrera resultat** och **skriver Set-Mailbox** i aktivitetsfilterrutan.

5. Välj en granskningspost i resultatet. Klicka på **Mer** information i den **utfällna menyn Information.** Du måste granska informationen för varje granskningspost för att avgöra om aktiviteten är relaterad till vidarebefordran av e-post.

   - **ObjectId:** Aliasvärdet för postlådan som ändrades.
   - **Parametrar:** _ForwardingSmtpAddress_ anger målets e-postadress.
   - **UserId:** Användaren som konfigurerade vidarebefordran av e-post för postlådan i **fältet ObjectId.**

Mer information finns i Fastställa [vem som har konfigurerat vidarebefordran av e-post för en postlåda.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
