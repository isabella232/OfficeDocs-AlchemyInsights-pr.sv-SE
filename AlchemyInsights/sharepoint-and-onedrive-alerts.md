---
title: Fördröjningar vid mottagning av SharePoint-och OneDrive-aviseringar
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785683"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Fördröjningar vid mottagning av SharePoint-och OneDrive-aviseringar

- Kontrol lera först skräppostmappen i e-postmeddelandet.
- Om **alla aviseringar från flera filer eller bibliotek är försenade**kan du gå till [instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home?ref=/servicehealth) för att söka efter eventuella rådgivare/händelser som kan komma att inträffa med SharePoint eller Exchange. Problemet kan bero på SharePoint-aviseringens kapacitet eller fördröjningar i e-postmeddelanden via Exchange. Observera även om andra e-postmeddelanden levereras – om det inte är det beror problemet sannolikt på Exchange-fördröjningar.
- Om **en enskild avisering från en viss fil eller ett visst bibliotek inte levereras**försöker du ta bort och återskapa den. Se [Hantera, Visa eller ta bort SharePoint-aviseringar](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) för att återskapa aviseringen.

> [!NOTE]
> - Det går inte att skicka aviseringar till en distributions grupp. Endast säkerhets-och O365-grupper stöds.
> - Du kan inte anpassa e-postmallar för aviseringar. Du måste använda Microsoft Flow eller SharePoint Designer-arbetsflöde för att få dem.
