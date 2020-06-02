---
title: Identifiera IP-adress och klient i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508934"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifiera IP-adress och klient i granskningsloggar

IP-adressen som motsvarar en aktivitet av en Microsoft 365-användare eller administratör visas i granskningsloggarna. Klientinformationen loggas också. Här är stegen för att identifiera sådan information

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå till söksidan **för sökfunktionen i**  >  **sökgranskning.**

   Om du är intresserad av en viss aktivitet väljer du den i **listan Aktiviteter.** Om inte, returneras alla aktiviteter för den valda användaren (standardinställning).

   **Obs:** Vissa aktiviteter kanske inte är tillgängliga i **menyn Aktiviteter.** Dessa granskningsobjekt returneras dock om **Visa resultat för alla aktiviteter** är markerat (standardinställning).

3. Ange användarnamnet i fältet **Användare,** välj lämpligt datumintervall för aktiviteten och klicka sedan på **Sök**.

I resultaten kan du se IP-adressen för den aktiviteten i resultatfönstret. Välj granskningsposten om du vill visa detaljerad information i **informationsutfällningen** (till exempel Klient, Användare som utförde åtgärden osv.).

Mer information finns [i Hitta IP-adressen för den dator som används för att komma åt ett komprometterat konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
