---
title: Problem med administratörsmedgivande
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952591"
---
# <a name="admin-consent-issues"></a>Problem med administratörsmedgivande

1. Aktivera [arbetsflödet för administratörsmedgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) för att tillåta användare att begära godkännande från administratören direkt från skärmen med medgivande.

1. Om du eller ditt programs användare ser oväntade fel under medgivandeprocessen läser du den här artikeln för felsökningssteg: Oväntat fel när användare utför medgivande [till ett program.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Läs mer om [administratörsmedgivande Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) hur medgivandeuppslag fungerar och hur du utvärderar en begäran om administratörsmedgivande [för hela klientorganisationen.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Program som integreras med Microsofts identitetsplattform följer en auktoriseringsmodell som ger användare och administratörer kontroll över hur data kan nås. Implementeringen av auktoriseringsmodellen har uppdaterats Microsofts identitetsplattform slutpunkten och den ändrar hur en app måste interagera med Microsofts identitetsplattform. Se [Behörigheter och medgivande i Microsofts identitetsplattform-slutpunkten](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) för en översikt över den här auktoriseringsmodellen, inklusive omfattningar, behörigheter och medgivande.