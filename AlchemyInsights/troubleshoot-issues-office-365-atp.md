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
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766763"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Felsöka problem med Office 365 ATP

- **Märker förseningar med e-postleverans?** Prova att använda alternativet Dynamisk leverans för dina ATP-principer för säkra bilagor. På så sätt undviker du förseningar i leveransen av e-postmeddelanden samtidigt som mottagare skyddas från skadliga filer.
- **Vill du rapportera falska positiva eller falska negativ?** Använd den här länken för att skicka in filen för analys:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Visste du att du kan aktivera ATP Safe Links skydd för e-post som skickas mellan personer i din organisation?** Gör så här:
    1. Gå https://protection.office.comtill och logga in.
    2. Gå till säkra > länkar för > **hothanteringspolicy****.** **Threat management**
    3. Redigera (eller lägga till) en princip under **Principer som gäller för specifika mottagare.**
    4. Välj **Använd säkra länkar till meddelanden som skickas inom organisationen**.
    5. Spara din princip och tillåt cirka 30 minuter för dina ändringar att arbeta sig igenom ditt datacenter.
- Mer hjälp med ATP finns i [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).