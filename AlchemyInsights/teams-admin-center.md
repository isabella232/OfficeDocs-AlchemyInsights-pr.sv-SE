---
title: Administrationscenter för Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670382"
---
# <a name="teams-admin-center"></a>Administrationscenter för Teams

Lär dig mer om hur du hanterar Teams med [Administrationscenter för Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Om du saknar åtkomst till Administrationscenter för Teams kontrollerar du följande:

- Att du har tillåtit lämpliga [IP-adresser och URL:er för Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på alla perimeterenheter (brandvägg osv.) eller i brandväggsreglerna på din lokala dator.
- Att inloggningen du använder för åtkomst till Administrationscenter för Teams matchar ditt användarnamn som visas i [administrationsportalen för Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Om användarna inte visas i Administrationscenter för Teams kontrollerar du följande:

- Har du skapat användare eller tilldelat licenser under de senaste 24 timmarna? Se till att vänta minst 24 timmar innan du skapar ett supportärende.
- Har du tilldelat lämpliga licenser?
- Om du har en lokal Active Directory-version kontrollerar du att [värdet för msRTCSIP-PrimaryUserAddress eller SIP-adressen i fältet ProxyAddresses i din lokala Active Directory är unikt och att formatet matchar](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**användar namn** från [administrations centret för Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Om du planerar att hålla en distribution av Skype för företag och låta användare vara lokalt anslutna och online: Följ instruktionerna för att **Konfigurera hybrid med Teams och Skype för företag – Online** i din Skype för företag-Server och flytta användare online.
