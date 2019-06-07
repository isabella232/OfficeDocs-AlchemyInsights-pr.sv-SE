---
title: Identifiera IP-adressen och klienten i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752077"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifiera IP-adressen och klienten i granskningsloggar

IP-adress som motsvarar en aktivitet av en användare eller administratör visas i granskningsloggarna. Klientinformation loggas också. Här är stegen för att identifiera sådan information

1. Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)

2. Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.

   Om du är intresserad av en viss aktivitet, markerar du den i listan **aktiviteter** . Annars returneras alla aktiviteter för den valda användaren (standardinställning).

   **Obs**: vissa aktiviteter kanske inte är tillgängliga i menyn **aktiviteter** . men de granska objekt returneras om **Visa resultat för alla aktiviteter** är markerad (standard).

3. Ange användarnamnet i fältet **användare** , Välj lämpligt datumintervall för aktiviteten och klicka sedan på **Sök**.

I resultatet ser du IP-adressen för den aktiviteten i resultatfönstret. Markera granskningsposten se detaljerad information i **information** utfällbar meny (t ex klient, användaren som utförde åtgärden osv.).

Mer information finns i [söka efter IP-adressen för den dator som används för åtkomst till eventuella skador](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
