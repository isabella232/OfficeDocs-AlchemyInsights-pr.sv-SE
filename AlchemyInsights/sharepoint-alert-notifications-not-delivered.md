---
title: SharePoint-aviseringarna har inte levererats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047085"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-aviseringarna har inte levererats

Vänligen kontrollera skräppostmappen i din e-post, eftersom ibland kan varningar gå dit.

Ta reda på om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.

- **Enskilda aviseringar levereras inte**: om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den. Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) för att återskapa aviseringen.
- **Alla aviseringar levereras inte**: om alla aviseringar från flera filer eller bibliotek inte levereras, gå till [instrumentpanelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att kontrollera om det finns några bulletiner/incidenter som kan inträffa med SharePoint eller Exchange. Problemet kan vara med SharePoint alert-funktionen eller fördröjningar i e-postmeddelanden via Exchange. Det kommer också att vara viktigt att notera om andra e-post levereras, och om inte, är problemet sannolikt med Exchange förseningar.

FAQ om varningar:

- Det går inte att skicka aviseringar till distributionsgruppen, endast säkerhets-och O365-grupper stöds.
- Du kan inte anpassa e-postmallar för notifieringar. Du måste använda Microsoft FLOW eller SharePoint Designer arbetsflöde för att uppnå dessa.

Mer information:

- **Aviseringsinställning**: Mer information om hur du ställer in aviseringar finns [i skapa en avisering för att få ett meddelande när en fil eller mapp ändras i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Felsöka aviseringar**: Mer information om felsökning av aviseringar finns i [användare får inte SharePoint Online varningsmeddelanden](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Avancerad O365-efterlevnad varnings principer**: Mer information om hur du ställer in dessa aviseringar finns i [efterlevnad aviserings principer](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **SharePoint och OneDrive granskningsloggar**: Mer information om hur du hämtar dessa händelser finns [i Sök i granskningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Aviseringar som skickas av Advanced Threat Protection**: se [ATP för SharePoint och OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Aviseringar som skickas av data förlust förebyggande principer**: se [e-POSTAVISERINGAR för DLP-principer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Närliggande ämnen

Vill du prova Microsoft Flow i SharePoint Online?

- [Skapa flöde](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint och Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
