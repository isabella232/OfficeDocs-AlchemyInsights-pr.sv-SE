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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831752"
---
# <a name="missing-emails-in-quarantine"></a>E-postmeddelanden saknas i karantän"

Administratörer kan [visa, släppa eller ta bort dessa meddelanden.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Om du vill öppna & Säkerhets- och efterlevnadscenter går du till [https://protection.office.com](https://protection.office.com/) . Om du vill öppna sidan Karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan söka efter följande värden:  

- **Meddelande-ID**: Meddelandets globalt unika identifierare. Om du markerar ett meddelande i listan visas värdet  **för Meddelande-ID**  i  **den**  utfällade rutan Information som visas. Administratörer kan använda [meddelandespårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) för att söka efter meddelanden med motsvarande värden för meddelande-ID.
- **Avsändarens e-postadress**: En enskild avsändarens e-postadress.
- **Mottagarens e-postadress**: En enskild mottagares e-postadress.
- **Ämne**: Använd meddelandets hela ämne. Sökningen är inte skiftlägeskänslig.

När du har angett sökvillkoren klickar du på ![ Uppdatera knappen Uppdatera ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **för** att filtrera resultatet.  

De cmdlets du använder för att visa och hantera meddelanden och filer i karantän är:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Observera att den här cmdleten endast används för meddelanden, inte för skadlig programvara från ATP för SharePoint Online, OneDrive för företag eller Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)