---
title: SharePoint aviseringsmeddelanden som inte levereras
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957919"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint aviseringsmeddelanden som inte levereras

Titta i skräppostmappen eftersom ibland kan aviseringar finnas där.

Avgöra om **alla aviseringar inte levereras eller** om en enskild **avisering** från en viss fil eller ett visst bibliotek inte levereras.

- **Enskilda aviseringar levereras inte:** Om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den. Mer [information finns i Hantera, visa SharePoint ta bort en avisering](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) om du vill återskapa aviseringen.
- **Alla aviseringar** levereras inte: Om alla aviseringar från flera [](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) filer eller bibliotek inte levereras kan du gå till hälsoinstrumentpanelen för att se om det finns rådgivningar/incidenter som SharePoint eller Exchange. Problemet kan vara med funktionen för SharePoint eller fördröjningar av e-postmeddelanden via Exchange. Det är också viktigt att observera om annan e-post levereras och om den inte levereras är problemet sannolikt Exchange fördröjningar.

Vanliga frågor och svar om aviseringar:

- Det går inte att skicka aviseringar till distributionsgruppen, det är bara säkerhets- och O365-grupper som stöds.
- Du kan inte anpassa aviseringsmallar för e-post. måste du använda Microsoft FLOW eller SharePoint Designer-arbetsflödet för att uppnå dem.

## <a name="related-topics"></a>Relaterade ämnen

Vill du prova Microsoft Flow i SharePoint Online?

- [Skapa Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint och Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
