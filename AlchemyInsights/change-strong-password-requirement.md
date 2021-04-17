---
title: Ändra krav på starkt lösenord
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818486"
---
# <a name="change-strong-password-requirement"></a>Ändra krav på starkt lösenord

Microsoft kräver starka lösenord som standard.

Med PowerShell kan du inaktivera starka lösenord för specifika användare med följande kommandon:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Om du vill inaktivera starka lösenord för alla användare använder du:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Mer information om lösenordsprincip](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Ansluta till Microsoft 365 med PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mer information om PowerShell MsolUser-kommandon](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
