---
title: Problem med Yammer-licenser
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657294"
---
# <a name="yammer-licensing-issues"></a>Problem med Yammer-licenser

Alla användare måste ha en licens för att använda Yammer Enterprise-tjänsten, men som standard är Yammer inte att användare har en licens för att få åtkomst till tjänsten. När en administratör ändrar inställningen för att blockera Microsoft 365-användare utan Yammer-licenser, får inte användare som inte har tilldelats Yammer-licenser åtkomst till Yammer-tjänsten. Mer information finns i [hantera användar licenser för Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

När licenser tas bort från användarna visas inte Yammer-panelen längre och andra tjänster kan använda licens borttagning för att dölja funktioner. I andra fall kan funktioner fortfarande visas men kräver tilldelning av licenser.  

**Licensen uppdateras inte för användaren**  

Ibland tilldelas en användare en licens men kan fortfarande inte komma åt Yammer. Det är ofta större att det uppstår fördröjningar när en Mass licens tilldelning pågår. Yammer-användare kanske inte uppdateras i samma ordning som licenser ändras i Azure AD eftersom systemet körs asynkront. Vänta 24 timmar innan du öppnar ett support ärende för att rapportera synkroniseringsproblem.  

**Tilldelning av Mass licenser**  

Licenser kan tilldelas via administrations centret eller PowerShell-skript. Mer information finns i [tilldela licenser till användare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) och [tilldela licenser till användar konton med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Support tillhandahåller inte hjälp med att skapa skript, men dokumentation i licens tilldelning för Yammer är tillgänglig. Mer information finns i [hantera Yammer-licenser med hjälp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).