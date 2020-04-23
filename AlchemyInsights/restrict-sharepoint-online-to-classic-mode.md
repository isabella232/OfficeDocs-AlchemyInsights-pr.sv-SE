---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742487"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begränsa SharePoint Online till klassiskt läge

Vissa organisationer kräver fortfarande upplevelsen av klassiskt läge. Även om det inte finns några planer på att ta bort klassiskt läge på detaljerad nivå, är det inte längre möjligt att begränsa en hel organisation (klient) till klassiskt läge för listor och bibliotek.

Administratören har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade opt-out-växlar som vi tillhandahåller på följande nivåer:

- webbplatssamling
- Webbplats
- Lista
- Bibliotek

Dessutom kommer listor som använder vissa funktioner och anpassningar som inte stöds av moderna fortfarande automatiskt att växlas till klassiskt läge.

Från och med den 1 april 2019 kommer processen att inaktivera klientnivå välja bort modern lista och bibliotek startar och fortsätter till och med 31 maj 2019.  Listorna och biblioteken som är i klassiskt läge som ett resultat av klientanmälan flyttas automatiskt till modernt.

Om du behöver klassiskt läge kan du se mer information [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP Powershell instruktion [här](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativ och verktyg som du kan använda idag för att använda det klassiska läget erfarenhet.
