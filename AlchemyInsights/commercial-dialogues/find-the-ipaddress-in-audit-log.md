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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483716"
---
# <a name="find-the-ip-address-in-audit-log"></a>Hitta IP-adressen i granskningsloggen

1. IP-adressen som motsvarar en aktivitet som utförts av en användare eller administratör visas i granskningsloggarna. Klientinformationen loggas också. Så här identifierar du IP-adressen:

1. Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök**  >  **[granskningsloggsökning.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultatet hämta data från tidigare datum.
1. Om du är intresserad av en viss aktivitet väljer du den i **aktivitetslistan.** annars returneras alla aktiviteter för den valda användaren som standard. Observera att vissa aktiviteter kanske inte är tillgängliga för markering från **menyn** Aktiviteter. Granskningsobjekten returneras emellertid om Visa resultat **för alla aktiviteter är** markerat (standardinställning).
1. Ange datumintervallet och välj **användarnamnet för** den användare du vill undersöka i fältet Användare.
1. Välj **Sök.** Aktiviteterna visas under **Resultat.** Du kan se IP-adressen för varje aktivitet.
1. Om du vill visa information väljer du en aktivitet och sedan **Mer information.**

Mer information finns i Söka i [Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)