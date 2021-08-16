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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017150"
---
# <a name="find-the-ip-address-in-audit-log"></a>Hitta IP-adressen i granskningsloggen

1. IP-adressen som motsvarar en aktivitet som utförts av en användare eller administratör visas i granskningsloggarna. Klientinformationen loggas också. Så här identifierar du IP-adressen:

1. Gå till [säkerhets- Office 365 för & säkerhets- och efterlevnadscenter.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök i**  >  **[granskningsloggsökning](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Om du är intresserad av en viss aktivitet väljer du den i **listan** Aktiviteter. Annars returneras alla aktiviteter som standard för den valda användaren. Observera att vissa aktiviteter kanske inte är tillgängliga i menyn **Aktiviteter.** Dessa granskningsobjekt returneras emellertid om **Visa resultat för alla aktiviteter** är markerat (standardinställning).
1. Ange datumintervallet och välj **användarnamnet för** den användare du vill undersöka i fältet Användare.
1. Välj **Sök**. Aktiviteterna visas under **Resultat.** Du kan se IP-adressen för varje aktivitet.
1. Om du vill visa information väljer du en aktivitet och sedan **Mer information.**

Mer information finns i Söka i Office 365 [granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)