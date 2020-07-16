---
title: Licensproblem med Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148427"
---
# <a name="yammer-licensing-issues"></a>Licensproblem med Yammer

Alla användare måste ha en licens för att använda Yammer Enterprise-tjänsten, men som standard kräver Yammer inte att användarna har licens att komma åt tjänsten. När en administratör ändrar inställningen för att blockera Microsoft 365-användare utan Yammer-licenser kan användare som inte har tilldelats en Yammer Enterprise-licens inte komma åt Yammer-tjänsten. Mer information finns [i Hantera Yammer-användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

När licenser tas bort från användare visas inte längre Yammer-panelen och andra tjänster kan använda licensborttagning för att dölja funktioner. I andra fall kan funktioner fortfarande visas men kräver licenstilldelning för att fungera.  

**Licensen uppdateras inte för användaren**  

Ibland tilldelas en användare en licens men kan fortfarande inte komma åt Yammer. Det är mer sannolikt att fördröjningar uppstår när en masslicenstilldelning pågår. Yammer-användare kanske inte uppdateras i samma ordning som licenser ändras i Azure AD eftersom systemet körs asynkront. Vänta upp till 24 timmar innan du öppnar ett supportärende för att rapportera problem med licenssynkronisering.  

**Tilldelning av bulklicenser**  

Licenser kan tilldelas via administrationscentret eller PowerShell-skript. Mer information finns i [Tilldela licenser till användare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) och Tilldela licenser till [användarkonton med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Support hjälper inte till att skapa skript, men dokumentation om Yammer-licenstilldelning är tillgänglig. Mer information finns i [Hantera Yammer-licenser med Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).