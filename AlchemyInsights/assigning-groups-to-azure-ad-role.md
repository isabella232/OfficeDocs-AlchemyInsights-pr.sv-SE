---
title: Tilldela grupper till Azure AD-roll
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
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036258"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tilldela grupper till Azure AD-roll

Så här tilldelar du en Azure AD-grupp med behörighetskälla i Azure AD till en Azure AD-roll:

1. Skapa en ny grupp – Så här skapar du en ny grupp:

    a. Logga in på administrationscentret för Azure AD med behörighet **som rolladministratör eller** **global administratörsbehörighet.**
    b. Välj **Azure Active Directory > Grupper > Alla grupper > Ny grupp**.
    c. Skapa gruppen.

2. Tilldela rollen till gruppen antingen när gruppen skapas eller när gruppen har skapats.

    a. Om du vill tilldela en roll till gruppen när gruppen skapas kan du aktivera växlingsknappen **Azure AD-roller** för gruppen och skapa gruppen.
    b. Om du vill tilldela en roll till gruppen  efter att den har skapats går du till fliken Tilldelade roller för den nya gruppen och tilldelar rollen till gruppen.  

**Hantera medlemskap för en grupp som har tilldelats Azure AD-roll**

För att förhindra ökning av behörigheter kan endast behöriga rolladministratörer och globala administratörer som standard ändra medlemskapet i en grupp som har tilldelats till en roll. De kan däremot välja att tilldela en ägare för en sådan grupp och delegera den här uppgiften.

Mer information om hur du tilldelar molngrupper till Azure AD-roller finns i [Tilldela en AD-roller till molngruppen.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Mer information om felsökning av roller som tilldelats molngrupper finns i [Felsöka roller tilldelade till molngrupper.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





