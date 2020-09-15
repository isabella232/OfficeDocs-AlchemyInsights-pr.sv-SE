---
title: Komma igång med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700725"
---
# <a name="workflows-in-sharepoint"></a>Arbets flöden i SharePoint

Om det inte går att skicka e-post från SharePoint-arbetsflöden kan din organisation ha påträffat begränsningar för Exchange Online-avsändaren.

Fel meddelandet "arbets flödet är upptaget" kan visas om du har något av följande:

- Du har ett arbets flöde i SharePoint Online som använder plattforms typen SharePoint 2010 eller SharePoint 2013 Workflow Platform.

- Arbets flödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.

När du kör arbets flödet skickas inte e-postmeddelandet, och du märker att fel meddelandet, att intern status är inaktive rad eller inte kan skicka till en mottagare visas.

Mer information finns i följande [artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

