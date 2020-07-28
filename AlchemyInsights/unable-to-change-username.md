---
title: Det går inte att ändra Användarnamn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440297"
---
# <a name="unable-to-change-username"></a>Det går inte att ändra Användarnamn

I vissa fall sprids inte UPN-ändringar (UserPrincipalName) till molnet. Valideringsfel kan visas i Office 365-portalen eller inte ändra användarnamnet eller e-postadressen. LÃ¶s problemet genom att ange UserPrincipalName manuellt med det här PowerShell-kommandot.

**Exempel: Byta namn på en användare**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Det här kommandot byter namn på davidc@contoso.com till davidchew@contoso.com.

Mer information finns i [Ange-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).