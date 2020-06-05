---
title: Förseningar i mottagandet av SharePoint- och OneDrive-aviseringar
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563528"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Förseningar i mottagandet av SharePoint- och OneDrive-aviseringar

- Kontrollera först mappen Skräppost eller Skräppost i din e-post.
- Om **alla aviseringar från flera filer eller bibliotek försenas**besöker du [instrumentpanelen För tjänsthälsan](https://portal.office.com/adminportal/home?ref=/servicehealth) för att kontrollera om det finns några råd/incidenter som kan uppstå med SharePoint eller Exchange. Problemet kan vara med SharePoint-varningsfunktionen eller fördröjningar i e-postmeddelanden via Exchange. Observera också om annan e-post levereras – om inte, är problemet sannolikt med valutakursförseningar.
- Om **en enskild avisering från en viss fil eller ett visst bibliotek inte levereras**försöker du ta bort och återskapa den. Se [Hantera, visa eller ta bort SharePoint-aviseringar](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.

> [!NOTE]
> - Aviseringar kan inte skickas till en distributionsgrupp. Endast säkerhets- och O365-grupper stöds.
> - Du kan inte anpassa aviseringsmallar för e-post. Du måste använda Microsoft Flow- eller SharePoint Designer Workflow för att uppnå dessa.
