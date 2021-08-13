---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958819"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begränsa SharePoint Online till klassiskt läge

Vissa organisationer måste fortfarande ha klassiskt läge. Det finns inga planer på att ta bort klassiskt läge på detaljnivå, men det går inte längre att begränsa en hel organisation (klientorganisation) till klassiskt läge för listor och bibliotek.

Administratören har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade avanmälningar som vi tillhandahåller på följande nivåer:

- webbplatssamling
- webbplats
- lista
- bibliotek

Dessutom kommer listor som använder vissa funktioner och anpassningar som inte stöds av modern fortfarande att växlas automatiskt till klassiskt läge.

Med början den 1 april 2019 kommer processen att inaktivera avaktiveringsnivån för modern lista och bibliotek att starta och fortsätta fram till den 31 maj 2019.  De listor och bibliotek som är i klassiskt läge på grund av avanmälning av klientorganisation flyttas automatiskt till moderna.

Om du behöver klassiskt läge kan du läsa [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) mer [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och i PnP Powershell-instruktionen här, som beskriver alternativ och verktyg som du kan använda idag för att använda det klassiska läget.
