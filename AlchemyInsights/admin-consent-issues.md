---
title: Problem med administratörs medgivande
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901513"
---
# <a name="admin-consent-issues"></a>Problem med administratörs medgivande

1. Aktivera [arbets flödet för administratörer](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) för att tillåta användare att begära administratörs godkännande direkt från medgivande skärmen.

1. Om du eller dina programs användare ser oväntade fel under medgivande processen läser du den här artikeln för fel söknings steg: [oväntat fel vid medgivande till ett program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Läs mer om [Administratörs medgivande på Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hur [medgivande meddelandet](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerar och hur du [utvärderar en begäran om klient medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Program som integreras med Microsoft Identity Platform följer en Authorization-modell som gör att användare och administratörer kan styra hur data nås. Implementeringen av auktoriserings modellen har uppdaterats på slut punkten för Microsoft Identity Platform och ändrar hur en app måste samverka med Microsofts identitets plattform. Se [behörigheter och medgivande i slut punkten för Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) för en översikt över den här verifierings modellen, inklusive omfattningar, behörigheter och medgivande.