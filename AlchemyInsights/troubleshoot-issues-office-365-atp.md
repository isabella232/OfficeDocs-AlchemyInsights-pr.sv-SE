---
title: Felsöka problem med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511130"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Felsöka problem med Office 365 ATP

- **Märker förseningar med e-postleverans?** Prova att använda alternativet Dynamisk leverans för dina ATP-principer för säkra bilagor. På så sätt undviker du förseningar i leveransen av e-postmeddelanden samtidigt som mottagare skyddas från skadliga filer.
- **Vill du rapportera falska positiva eller falska negativ?** Använd den här länken för att skicka in filen för analys:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Visste du att du kan aktivera ATP Safe Links skydd för e-post som skickas mellan personer i din organisation?** Gör så här:
    1. Gå till https://protection.office.com och logga in.
    2. Gå till säkra länkar **för**  >  **Policy**  >  **hothanteringspolicy .**
    3. Redigera (eller lägga till) en princip under **Principer som gäller för specifika mottagare.**
    4. Välj **Använd säkra länkar till meddelanden som skickas inom organisationen**.
    5. Spara din princip och tillåt cirka 30 minuter för dina ändringar att arbeta sig igenom ditt datacenter.
- Mer hjälp med ATP finns i [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).