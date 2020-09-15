---
title: E-postmeddelanden som saknas i karantän
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673732"
---
# <a name="missing-emails-in-quarantine"></a>E-postmeddelanden som saknas i karantän "

Administratörer kan [Visa, frigöra eller ta bort dessa meddelanden.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Om du vill öppna säkerhets & Compliance Center går du till [https://protection.office.com](https://protection.office.com/) . Om du vill öppna sidan karantän direkt går du till [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan söka efter följande värden:  

- **Meddelande-ID**: Meddelandets globalt unika identifierare. Om du väljer ett meddelande i listan visas värdet för  **meddelande-ID**  i fönstret  **detaljerad information**  . Administratörer kan använda [meddelandespårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) för att söka efter meddelanden med motsvarande värden för meddelande-ID.
- **Avsändarens e-postadress**: En enskild avsändarens e-postadress.
- **Mottagarens e-postadress**: En enskild mottagares e-postadress.
- **Ämne**: Använd meddelandets hela ämne. Sökningen är inte skiftlägeskänslig.

När du har angett Sök villkoren klickar du på ![ uppdatera knappen uppdatera ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** för att filtrera resultaten.  

De cmdlets som du använder för att visa och hantera meddelanden och filer i karantänen är:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Exportera-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- För [hands version – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Observera att denna cmdlet endast gäller för meddelanden, inte malware-filer från ATP för SharePoint Online, OneDrive för företag eller teams.
- [Utgivning-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)