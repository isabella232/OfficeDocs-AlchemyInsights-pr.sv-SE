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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539842"
---
# <a name="missing-emails-in-quarantine"></a>E-postmeddelanden saknas i karantän"

Administratörer kan [visa, släppa eller ta bort dessa meddelanden.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Om du vill öppna & Säkerhets- och efterlevnadscenter går du till [https://protection.office.com](https://protection.office.com/) . Om du vill öppna sidan Karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan söka efter följande värden:  

- **Meddelande-ID**: Meddelandets globalt unika identifierare. Om du markerar ett meddelande i listan visas värdet  **för Meddelande-ID**  i  **den**  utfällade rutan Information som visas. Administratörer kan använda [meddelandespårning](/microsoft-365/security/office-365-security/message-trace-scc) för att söka efter meddelanden med motsvarande värden för meddelande-ID.
- **Avsändarens e-postadress**: En enskild avsändarens e-postadress.
- **Mottagarens e-postadress**: En enskild mottagares e-postadress.
- **Ämne**: Använd meddelandets hela ämne. Sökningen är inte skiftlägeskänslig.

När du har angett sökvillkor klickar du på ![knappen Uppdatera](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Uppdatera**, så filtreras resultatet.

De cmdlets du använder för att visa och hantera meddelanden och filer i karantän är:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Observera att den här cmdleten endast används för meddelanden, inte för skadlig programvara från Microsoft Defender för Office 365 för SharePoint Online, OneDrive för företag och Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)