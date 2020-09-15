---
title: Identifiera IP-adress och klient i gransknings loggar
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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668328"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifiera IP-adress och klient i gransknings loggar

Den IP-adress som motsvarar en aktivitet av en Microsoft 365-användare eller-administratör visas i gransknings loggarna. Klient informationen loggas också. Här är de här stegen för att identifiera sådan information

1. Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå till sidan **Sök**  >  **gransknings loggs sökning** .

   Om du är intresse rad av en viss aktivitet väljer du den i listan **aktiviteter** . Annars returneras alla aktiviteter för den valda användaren (standardinställningen).

   **Obs!** vissa aktiviteter kanske inte är tillgängliga i menyn **aktiviteter** . dessa gransknings objekt returneras emellertid om **Visa resultat för alla aktiviteter** är markerat (standardinställningen).

3. Ange användar namnet i fältet **användare** , Välj lämpligt datum intervall för aktiviteten och klicka sedan på **Sök**.

I resultatet kan du se IP-adressen för den aktiviteten i resultat fönstret. Välj gransknings posten för att se detaljerad information om utfällbar **information** (till exempel klient, användare som utförde åtgärder osv.).

Mer information finns i [hitta IP-adressen för datorn som används för att komma åt ett komprometterat konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
