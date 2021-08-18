---
title: Hitta IP-adressen i granskningsloggen
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902278"
---
# <a name="find-the-ip-address-in-audit-log"></a>Hitta IP-adressen i granskningsloggen

IP-adressen som motsvarar en aktivitet som utförts av en användare eller administratör visas i granskningsloggarna. Klientinformationen loggas också. Så här identifierar du IP-adressen:

1. Gör något av följande:
   - I den Microsoft 365 Efterlevnadscenter går <https://compliance.microsoft.com> du till **Lösningsgranskning.** \>  Du kan också använda om du vill **gå direkt** till sidan <https://compliance.microsoft.com/auditlogsearch> Granskning.
   - I Microsoft 365 Defender på <https://security.microsoft.com> går du till **Granska**. Du kan också använda om du vill **gå direkt** till sidan <https://security.microsoft.com/auditlogsearch> Granskning.

    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.

2. På sidan **Granska** kontrollerar du att **fliken Sök** är markerad och konfigurerar sedan följande inställningar:
   - **Datum och tidsintervall:** Välj datum/tid i **rutorna Start** **och** Slut.
   - **Aktiviteter**: Om du är intresserad av en viss aktivitet väljer du den i listan. Annars returneras **standardvärdet Visa resultat för alla** aktiviteter. Observera att vissa aktiviteter kanske inte är tillgängliga för markering. Dessa granskningsobjekt returneras emellertid om **Visa resultat för alla aktiviteter** är markerat.
   - **Användare:** Acceptera det tomma standardvärdet för att returnera resultat för alla användare, eller ange en eller flera användare.

3. När du är klar klickar du på **Sök**. Aktiviteterna visas på den nya **sidan Granskningssökning.**

4. I resultatet klickar du på **Filtrera resultat** och **skriver Set-Mailbox** i aktivitetsfilterrutan.

5. Välj en granskningspost i resultatet för att öppna den **utfällade** informationen.

Mer information finns i Söka i [granskningsloggen för att undersöka vanliga supportproblem.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
