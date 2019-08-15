---
title: SharePoint-aviseringar inte levereras
ms.author: efrene
author: efrene
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
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404820"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-aviseringar inte levereras

Kontrollera mappen Skräppost i ditt e-postmeddelande som aviseringar kan ibland gå dit.

Ta reda på om **alla notifieringar inte levereras** eller om **ett enskilt meddelande** från en specifik fil eller biblioteket inte har levererats.

- **Enskilda meddelanden levereras inte**: om en enskild avisering från en specifik fil eller biblioteket inte levereras, du kan försöka ta bort och återskapa den. Se [Hantera, visa, eller ta bort avisering](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) att skapa aviseringen.
- **Alla notifieringar inte levereras**: Besök [tjänsten hälsa instrumentpanelen](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för alla rekommendationerna/händelser som sker med SharePoint- eller om alla aviseringar från flera filer och bibliotek inte har levererats. Problemet kan bero på SharePoint alert kapacitet eller fördröjningar i e-postmeddelanden via Exchange. Det blir också viktigt att notera om annan e-post levereras och inte problemet sannolikt på förseningar i Exchange.

Vanliga frågor och svar om aviseringar:

- Det är inte möjligt att skicka aviseringar till distributionsgruppen endast säkerhet och O365 grupper stöds.
- Du kan inte anpassa alert e-mallar. Du måste använda Microsoft FLOW eller arbetsflödet i SharePoint Designer för att uppnå de.

Mer Information:

- **Notifieringsinställningar**: Mer information om hur du ställer in notifieringar finns i [Skapa en avisering om du vill bli meddelad när en fil eller mapp ändras i SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Felsöka varningar**: Mer information om felsökning av meddelanden finns i [användare får inte SharePoint Online aviseringar](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).
- **Avancerade O365 överensstämmelse Alert principer**: Mer information om hur du konfigurerar dessa aviseringar finns i [Alert principer för överensstämmelse](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).
- **SharePoint och OneDrive granska loggar**: Mer information om hur du hämtar dessa händelser finns i [söka granskningsloggen](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Meddelanden som skickas av Advanced Threat Protection**: finns [tillgängligt att LOVA för SharePoint och OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Principer för notifieringar som skickas av förhindra dataförlust**: se [e-postmeddelanden för DLP-principer](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Närliggande information

Vill du prova Microsoft Flow i SharePoint Online?

- [Skapa flöde](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint och flöde](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
