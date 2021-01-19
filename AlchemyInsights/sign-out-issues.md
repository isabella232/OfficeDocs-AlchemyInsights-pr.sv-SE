---
title: Problem med inloggning
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901300"
---
# <a name="sign-out-issues"></a>Problem med inloggning

Så här löser du problem med utloggning:

1. Om du eller en användare loggar in eller utsätts utanför program följer du anvisningarna i artiklarna [Konfigurera hantering av autentiseringsprocess med villkorsstyrd åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) eller [konfigurerbara tokens för token i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. De flesta andra problem med utloggning kan lösas genom att felsöka integreringen av Azure Active Directory (Azure AD) med det specifika programmet. Du hittar vägledning för en viss integrering genom att gå till den här [samlingen med själv studie kurser för att integrera program med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), inklusive:
    - SaaS program själv studie kurser
    - Självstudier för enkel inloggning
    - Själv studie kurser för användare