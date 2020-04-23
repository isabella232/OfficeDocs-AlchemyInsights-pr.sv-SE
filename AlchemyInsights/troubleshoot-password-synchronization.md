---
title: Felsöka lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732528"
---
# <a name="troubleshoot-password-synchronization"></a>Felsöka lösenordssynkronisering

Så här felsöker du problem där inga lösenord synkroniseras med Azure AD Connect version 1.1.614.0 eller senare:
  
1. Öppna en ny Windows PowerShell-session på Din Azure AD Connect-server med alternativet **Kör som administratör.**

2. Kör **Obegränsad set-executionPolicy-fjärrsignerad** eller **Ange körningspolicy.**

3. Starta Azure AD Connect-guiden.

4. Navigera till sidan **Ytterligare uppgifter,** välj **Felsöka**och klicka på **Nästa**.

5. På sidan Felsökning klickar du på **Starta för att starta felsökningsmenyn** i PowerShell.

6. Välj **Felsök lösenordssynkronisering**på huvudmenyn .

7. På undermenyn väljer du **Lösenordssynkronisering fungerar inte alls**.

**Förstå resultatet av felsökningsuppgiften**
  
Felsökningsuppgiften utför följande kontroller:
  
- Verifierar att lösenordssynkroniseringsfunktionen är aktiverad för din Azure AD-klientorganisation.

- Verifierar att Azure AD Connect-servern inte är i mellanlagringsläge.

- För varje befintlig lokal Active Directory-anslutning (som motsvarar en befintlig Active Directory-skog):

- 
  - Verifierar att lösenordssynkroniseringsfunktionen är aktiverad.

  - Söker efter pulsslagshändelser för lösenordssynkronisering i windows-programhändelseloggarna.

  - För varje Active Directory-domän under den lokala Active Directory-anslutningen:

  - Verifierar att domänen kan nås från Azure AD Connect-servern.

  - Verifierar att AD DS-konton (Active Directory Domain Services) som används av den lokala Active Directory-anslutningen har rätt användarnamn, lösenord och behörigheter som krävs för lösenordssynkronisering.

Mer hjälp med felsökning av lösenordssynkronisering finns i [Felsöka lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  