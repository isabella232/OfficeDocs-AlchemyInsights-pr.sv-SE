---
title: Administrationscenter för Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354106"
---
# <a name="teams-admin-center"></a>Administrationscenter för Teams

Lär dig mer om hur du hanterar Teams med [Administrationscenter för Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Om du saknar åtkomst till Administrationscenter för Teams kontrollerar du följande:

- Att du har tillåtit lämpliga [IP-adresser och URL:er för Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alla perimeterenheter (brandvägg osv.) eller i brandväggsreglerna på din lokala dator.
- Att inloggningen du använder för åtkomst till Administrationscenter för Teams matchar ditt användarnamn som visas i [administrationsportalen för Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Om användarna inte visas i Administrationscenter för Teams kontrollerar du följande:

- Har du skapat användare eller tilldelat licenser under de senaste 24 timmarna? Se till att vänta minst 24 timmar innan du skapar ett supportärende.
- Har du tilldelat lämpliga licenser?
- Om du har en lokal Active Directory kontrollerar du att värdet för [msRTCSIP-PrimaryUserAddress eller SIP-adressen i fältet ProxyAddresses i den lokala Active Directory är unikt och formatet matchar](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Användarens användarnamn** från Microsoft [365-administrationscentret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Om du tänker behålla en Skype för företag-server-distribution och låta användarna vara lokalt och online hemma: följ **"Konfigurera hybrid med Teams och Skype för företag – Online"** på kontrollpanelen för Skype för företag Server och flytta användarna online.
