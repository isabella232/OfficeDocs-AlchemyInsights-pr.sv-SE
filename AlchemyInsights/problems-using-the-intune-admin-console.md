---
title: Problem med att använda Administratörskonsolen Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555879"
---
# <a name="problems-using-the-intune-admin-console"></a>Problem med att använda Administratörskonsolen Intune

**"Åtkomst nekad" när du navigerar i Intune-administratörsportalen.**

- Om du är medlem i en anpassad Intune-roll kontrollerar du att en EMS-licens (Intune eller Enterprise Mobility Suite) har tilldelats ditt konto.
- Om du använder Configuration Manager för att hantera enheter kontrollerar du att du inte ingår i Intune-användarsamlingen för Configuration Manager MDM.
- Kontrollera att du har tilldelats lämpliga rollbaserade administrationskontroll (RBAC) behörigheter i Intune roller bladet.
- Kontrollera att gruppen som används inte är en distributionslista. Intune i Azure-portalen stöder endast användarkonton som tillhör Azure Active Directory-säkerhetsgrupper. Granska dina grupper i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.

**Användaren har för många behörigheter för tilldelad Intune-roll**

Råda användaren att gå till **Intune**  >  **Intune-roller**  >  **Mina behörigheter**  >  **Exportera** för granskning av beviljade behörigheter.

**Jag har lagt till en scopegrupp i en roll, men användare i den rollen ser fortfarande andra användare eller enheter.**

Scopegrupper filtrerar inte bort användare eller enheter. Scopegrupper:

- Begränsa vem användare kan tilldela principer eller program till.
- Tillåt endast specifika användare att köra fjärraktiviteter på enheter.

Mer information om scopegrupper finns i [Rollbaserad åtkomstkontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Jag har lagt till en användare i en Intune-roll, men de har fortfarande full åtkomst till Intune-administratörskonsolen.**

Navigera till Intune > **användare** i Azure-portalen och kontrollera att användaren inte har tilldelats någon av följande roller i Azure-portalen:

- Global administratör
- Tjänstadministratör för Intune
- SharePoint-administratör

Mer information finns i [Rollbaserad åtkomstkontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problem med åtkomst**

Mer information finns [i Du kan inte logga in på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).