---
title: Tilldela roller till Azure AD-rollen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885399"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tilldela roller till Azure AD-rollen

Så här tilldelar du en Azure AD-grupp med auktoritets källan i Azure AD till en Azure AD-roll:

1. Skapa en ny grupp – för att skapa en ny grupp:

    a. Logga in på administrations centret för Azure AD med **Administratörs** behörighet för administratörer eller **Global administratör** .
    b. Välj **> grupper i Azure Active Directory > alla grupper > ny grupp**.
    c. Skapa gruppen.

2. Tilldela rollen till gruppen antingen när grupp skapas eller efter att gruppen har skapats.

    a. Om du vill tilldela en roll till gruppen när du skapar en grupp kan du byta till gruppen och skapa gruppen med växla mellan **Azure AD-rollerna** .
    b. Om du vill tilldela en roll till gruppen efter att den har skapats navigerar du till fliken **tilldelade roller** för den nya gruppen och tilldelar rollen till gruppen.  

**Hantera medlemskap för en grupp som är tilldelad Azure AD-rollen**

För att förhindra behörighets höjning, kan endast privilegierade roll administratörer och globala administratörer ändra medlemskap för en grupp som är tilldelad en roll. De kan välja att tilldela en ägare för en sådan grupp och delegera uppgiften.

Mer information om hur du tilldelar moln grupper till Azure AD-roller finns i [tilldela en AD-roll till moln gruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Mer information om hur du felsöker roller tilldelade till moln grupper finns i [Felsöka roller som är tilldelade till moln grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





