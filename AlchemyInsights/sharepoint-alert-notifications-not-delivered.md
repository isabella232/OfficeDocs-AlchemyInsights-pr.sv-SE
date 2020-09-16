---
title: SharePoint-aviseringar skickas inte
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
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751261"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-aviseringar skickas inte

Kontrol lera mappen skräp post i e-postmeddelandet, så snart meddelanden kan komma dit.

Avgöra om **alla aviseringar inte levereras** eller om **en enskild avisering** från en viss fil eller ett visst bibliotek inte levereras.

- **Enskilda meddelanden levereras inte**: om en enskild avisering från en viss fil eller ett visst bibliotek inte levereras kan du försöka ta bort och återskapa den. Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.
- **Alla notifieringar levereras inte**: om alla aviseringar från flera filer eller bibliotek inte levereras kan du gå till [instrument panelen för tjänstens hälsa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) för att söka efter eventuella rådgivare/händelser som kan komma att inträffa med SharePoint eller Exchange. Problemet kan uppstå med aviserings kapaciteten för SharePoint eller fördröjningar i e-postmeddelanden via Exchange. Det är också viktigt att notera om andra e-postmeddelanden levereras och om så inte är fallet beror problemet sannolikt på Exchange-fördröjningar.

Vanliga frågor och svar:

- Det går inte att skicka meddelanden till distributions gruppen, endast säkerhets-och O365-grupper stöds.
- Du kan inte anpassa e-postmallar för aviseringar; Du måste använda Microsoft FLOW eller SharePoint Designer-arbetsflöde för att få dem.

## <a name="related-topics"></a>Relaterade ämnen

Vill du prova Microsoft Flow i SharePoint Online?

- [Skapa flöde](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint och flöde](https://flow.microsoft.com//blog/sharepoint-and-flow/)
