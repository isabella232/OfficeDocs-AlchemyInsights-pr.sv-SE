---
title: E-postmeddelanden saknas i karantän
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
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892065"
---
# <a name="missing-emails-in-quarantine"></a>E-postmeddelanden saknas i karantän

Administratörer kan [visa, släppa eller ta bort dessa meddelanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Gå till Microsoft 365 Defender i <https://security.microsoft.com> portalen på **.** \>  Eller använd för att gå direkt **till** sidan <https://security.microsoft.com/quarantine> Karantän.  

Mer information om de sök-/filtervärden du kan använda finns i Hantera meddelanden i karantän och filer [som administratör i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

De cmdlets som du använder för att visa och hantera meddelanden och filer i karantän är:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Observera att den här cmdleten endast är till för meddelanden, inte filer från Valv Bifogade filer för SharePoint, OneDrive eller Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
