---
title: Ändra krav på starkt lösenord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706579"
---
# <a name="change-strong-password-requirement"></a>Ändra ett starkt lösenordskrav

Microsoft kräver starka lösenord som standard. 

Med PowerShell kan du inaktivera starka lösenord för specifika användare med det här kommandot:<br>
*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*

- [Mer information om lösenordspolicy](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Ansluta till Microsoft 365 med PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Mer information om PowerShell MsolUser-kommandon](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
