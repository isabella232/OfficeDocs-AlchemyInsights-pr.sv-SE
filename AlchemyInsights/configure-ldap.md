---
title: Konfigurera LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885579"
---
# <a name="configure-ldap"></a>Konfigurera LDAP

Så här konfigurerar du LDAP:

1. Kontrol lera din domäns hälsa på [Azure-portalen](https://aka.ms/aadds-health).
1. Se till att det finns en giltig Azure AD-prenumeration och Azure AD Domain Services har Aktiver ATS.
1. Det certifikat som krävs för att aktivera säker LDAP måste erhållas från en betrodd offentlig certifikat utfärdare eller vara ett självsignerat certifikat.
1. Kontrol lera att certifikatet följer de nödvändiga [rikt linjerna](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ogiltigt certifikat**
1. Om du vill förnya ett certifikat följer du stegen för att skapa ett nytt certifikat och laddar upp det igen: [Konfigurera LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Information om hur du löser kända problem med säkra LDAP-aviseringar i Azure Active Directory Domain Services finns i [lösa LDAP-varningar](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
