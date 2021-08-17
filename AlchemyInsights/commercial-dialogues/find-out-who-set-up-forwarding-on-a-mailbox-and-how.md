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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895197"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ta reda på vem som har ställt in vidarebefordran för en postlåda och hur

Om extern vidarebefordran har angetts för en postlåda granskas aktiviteten som en del av **cmdleten Set-Mailbox.** Så här hittar du aktiviteten i granskningsloggen:

1. Gör något av följande:
   - I den Microsoft 365 Efterlevnadscenter går <https://compliance.microsoft.com> du till **Lösningsgranskning.** \>  Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - I Microsoft 365 Defender på <https://security.microsoft.com> går du till **Granska**. Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

   > [!NOTE]
   > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

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
