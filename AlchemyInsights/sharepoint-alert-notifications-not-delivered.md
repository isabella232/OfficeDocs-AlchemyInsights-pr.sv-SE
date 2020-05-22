---
title: Aviseringar om SharePoint-aviseringar har inte levererats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343077"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Aviseringar om SharePoint-aviseringar har inte levererats

Kontrollera SKRÄP-mappen i din e-post, eftersom varningar ibland kan gå dit.

Ta reda på om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.

- **Enskilda aviseringar levereras inte**: Om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den. Se [Hantera, visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.
- **Alla aviseringar levereras inte:** Om alla aviseringar från flera filer eller bibliotek inte levereras besöker du [instrumentpanelen för tjänstens hälsotillstånd](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att kontrollera om det finns några råd/incidenter som kan inträffa med SharePoint eller Exchange. Problemet kan vara med SharePoint-varningsfunktionen eller fördröjningar i e-postmeddelanden via Exchange. Det kommer också att vara viktigt att notera om andra e-postmeddelanden levereras, och om inte, är problemet sannolikt med Exchange förseningar.

Vanliga frågor och svar om varningar:

- Det går inte att skicka aviseringar till distributionsgrupp, endast säkerhets- och O365-grupper stöds.
- Du kan inte anpassa aviseringsmallar för e-post. Du måste använda Microsoft FLOW eller SharePoint Designer Workflow för att uppnå dessa.

## <a name="related-topics"></a>Relaterade ämnen

Vill du prova Microsoft Flow i SharePoint Online?

- [Skapa flöde](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint och flöde](https://flow.microsoft.com//blog/sharepoint-and-flow/)
