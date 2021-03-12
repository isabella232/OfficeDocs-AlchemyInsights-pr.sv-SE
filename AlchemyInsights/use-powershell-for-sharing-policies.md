---
title: Använda Windows PowerShell för delningsprinciper och organisationsrelationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709484"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Använda Windows PowerShell för delningsprinciper och organisationsrelationer


Information om organisationsrelationer finns i den detaljerade informationen om syntax och parametrar för: [Hämta federationsinformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Ny organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Ange organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  och  [Ta bort organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

För att skapa delningsprinciper, gå till [Ny delningsprincip](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). För att  [tillämpa en delningsprincip på en postlåda eller användare](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  måste du använda en kombination av  [Ange postlåda](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) och [Hämta postlåda](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nya principen. För att  [ändra, inaktivera eller ta bort en delningsprincip](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  måste du använda  [Ange delningsprincip](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) och [Ta bort delningsprincip](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Mer information för fullständig förståelse av det här avsnittet finns här:**

[Delning i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)