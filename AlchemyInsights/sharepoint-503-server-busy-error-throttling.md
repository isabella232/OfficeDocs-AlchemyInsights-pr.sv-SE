---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048634"
---
# <a name="sharepoint-online-throttling"></a>Begränsning av SharePoint Online

Användare kan få en 503 Server är upptagen fel när du försöker navigera till SharePoint eller OneDrive webbplatser. 

Det här felet kan orsakas av begränsning i SharePoint-tjänsten. SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet för SharePoint Online-tjänsten. Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser. Om du inte blir begränsad, 99% av tiden är det på grund av anpassad kod.

Mer information om begränsning se, [undvika att få begränsas eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Om du tror att det här felet inte är relaterat till begränsning, kan du kontrollera om det finns aktivt underhåll som inträffar på din klient genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/MessageCenter).

 Slutligen, se till att du besöker sidan för [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth) för att kontrollera eventuella bulletiner/incidenter som kan inträffa.

