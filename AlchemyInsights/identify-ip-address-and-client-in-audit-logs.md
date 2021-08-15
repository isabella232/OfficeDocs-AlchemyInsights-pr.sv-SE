---
title: Identifiera IP-adress och klient i granskningsloggar
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014918"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifiera IP-adress och klient i granskningsloggar

IP-adressen som motsvarar en aktivitet av en Microsoft 365 användare eller administratör visas i granskningsloggarna. Klientinformationen loggas också. Här är stegen för att identifiera sådan information

1. Logga in på [Microsoft 365 Kompatibilitetscenter.](https://protection.office.com/)

2. Gå till sidan **Sök**  >  **granskningsloggsökning.**

   Om du är intresserad av en viss aktivitet väljer du den i **listan** Aktiviteter. Om det inte är markerat returneras alla aktiviteter för den valda användaren (standardinställning).

   **Obs!** Vissa aktiviteter kanske inte är tillgängliga på **menyn** Aktiviteter. Dessa granskningsobjekt returneras emellertid om **Visa resultat för alla aktiviteter** är markerat (standardinställning).

3. Ange användarnamnet i **fältet Användare,** välj lämpligt datumintervall för aktiviteten och klicka sedan på **Sök**.

I resultatet visas IP-adressen för aktiviteten i resultatfönstret. Välj granskningsposten om du  vill se detaljerad information i den utfällna informationen (till exempel Klient, Användare som utfört en åtgärd osv.).

Mer information finns i Hitta [IP-adressen för datorn som används för att komma åt ett komprometterat konto.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
