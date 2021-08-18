---
title: Ta reda på vem som har ställt in vidarebefordran för en postlåda och hur
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317826"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ta reda på vem som har ställt in vidarebefordran för en postlåda och hur

Om extern vidarebefordran har angetts för en postlåda granskas aktiviteten som en del av **cmdleten Set-Mailbox.** Så här hittar du aktiviteten i granskningsloggen:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till  \> **Lösningsgranskning.** Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen .  Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

   **Obs!** Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

2. På sidan **Granska** kontrollerar du att **fliken Sök** är markerad och konfigurerar sedan följande inställningar:
   - Välj datum-/tidsintervallet i **rutorna Start** **och** Slut.
   - Kontrollera att **rutan** Aktiviteter innehåller **Visa resultat för alla aktiviteter.**

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. I resultatet klickar du på **kolumnen Aktivitet** för att sortera resultatet och letar efter **Set-Mailbox-poster.**

5. Välj en aktivitet i resultatet för att öppna den utfällade informationen. Du måste granska informationen för varje granskningspost för att avgöra om aktiviteten är relaterad till vidarebefordran av e-post:
   - **ObjectId:** Aliasvärdet för postlådan som ändrades.
   - **Parametrar:** _ForwardingSmtpAddress_ anger målets e-postadress.
   - **UserId:** Användaren som konfigurerade vidarebefordran av e-post för postlådan i **fältet ObjectId.**

Mer information finns i Fastställa [vem som har konfigurerat vidarebefordran av e-post för en postlåda.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
