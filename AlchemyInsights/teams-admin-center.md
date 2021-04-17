---
title: Administrationscenter för Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826397"
---
# <a name="teams-admin-center"></a>Administrationscenter för Teams

Lär dig mer om hur du hanterar Teams med [Administrationscenter för Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Om du saknar åtkomst till Administrationscenter för Teams kontrollerar du följande:

- Att du har tillåtit lämpliga [IP-adresser och URL:er för Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alla perimeterenheter (brandvägg osv.) eller i brandväggsreglerna på din lokala dator.
- Att inloggningen du använder för åtkomst till Administrationscenter för Teams matchar ditt användarnamn som visas i [administrationsportalen för Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Om användarna inte visas i Administrationscenter för Teams kontrollerar du följande:

- Har du skapat användare eller tilldelat licenser under de senaste 24 timmarna? Se till att vänta minst 24 timmar innan du skapar ett supportärende.
- Har du tilldelat lämpliga licenser?
- Om du har en lokal Active Directory kontrollerar du att värdet för [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) eller SIP-adressen i fältet ProxyAddresses i din lokala Active Directory är unikt och formatet matchar **sip:** Användarens användarnamn från administrationscentret för [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Om du har för avsikt att behålla en Skype för företag – Server-distribution och låta användarna vara lokalt uppkopplade och online: följ **"Konfigurera hybrid** med Teams och Skype för företag – Online" i Skype för företag – Server-kontrollpanelen och flytta användare online.
