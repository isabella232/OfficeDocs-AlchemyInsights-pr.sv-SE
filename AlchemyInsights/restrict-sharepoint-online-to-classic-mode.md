---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752086"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begränsa SharePoint Online till klassiskt läge

Vissa organisationer kräver fortfarande den klassiska läges upplevelsen. Det finns inga planer på att ta bort klassiskt läge på en detaljerad nivå, men det är inte längre möjligt att begränsa en hel organisation (klient) till klassiskt läge för listor och bibliotek.

Administratören kommer att ha följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade opt-out-växlar som vi tillhandahåller på följande nivåer:

- webbplatssamling
- Webbplats
- Lista
- Bibliotek

Dessutom växlar listor som använder vissa funktioner och anpassningar som inte stöds av modern fortfarande automatiskt till klassiskt läge.

Från och med den 1 april 2019, processen för att inaktivera klientnivå välja bort moderna listan och bibliotek startar och fortsätter genom den 31 maj 2019.  Listor och bibliotek som är i klassiskt läge som ett resultat av arrendator opt-out kommer automatiskt att flyttas till modern.

Om du behöver klassiskt läge se mer information [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP PowerShell-instruktion [här](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativ och verktyg som du kan använda i dag för att använda klassisk mode-upplevelse.
