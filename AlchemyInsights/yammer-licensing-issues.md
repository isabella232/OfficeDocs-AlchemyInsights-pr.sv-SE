---
title: Yammer licensproblem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989753"
---
# <a name="yammer-licensing-issues"></a>Yammer licensproblem

Alla användare måste ha en licens för att använda Yammer Enterprise-tjänsten, men Yammer kräver som standard inte att användarna har en licens för att få åtkomst till tjänsten. När en administratör ändrar inställningen för att blockera Microsoft 365 användare utan Yammer-licenser kan användare som inte har tilldelats en Yammer Enterprise-licens inte komma åt Yammer tjänsten. Mer information finns i [Hantera Yammer användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

När licenser tas bort från användare visas Yammer visas inte längre och andra tjänster kan använda licensborttagning för att dölja funktioner. I andra fall kan funktioner fortfarande visas, men det kan krävas licenstilldelning för att fungera.  

**Licensen uppdateras inte för användaren**  

Ibland tilldelas en användare en licens men kan fortfarande inte komma åt Yammer. Fördröjningar är mer troliga när en masslicenstilldelning pågår. Yammer användare kanske inte uppdateras i samma ordning som licenser ändras i Azure AD eftersom systemet körs asynkront. Vänta upp till 24 timmar innan du öppnar ett supportärenden för att rapportera synkroniseringsproblem för licenser.  

**Masslicenstilldelning**  

Licenser kan tilldelas via administrationscentret eller PowerShell-skript. Mer information finns i [Tilldela licenser till användare och](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Tilldela licenser till [användarkonton med Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoft Support ger inte hjälp med att skapa skript, men dokumentation Yammer om licenstilldelning finns tillgänglig. Mer information finns i Hantera [Yammer med hjälp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).