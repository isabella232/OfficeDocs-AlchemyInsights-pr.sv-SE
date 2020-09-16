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
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751441"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begränsa SharePoint Online till klassiskt läge

Vissa organisationer kräver fortfarande klassiskt läge. Även om det inte finns några planer att ta bort klassiskt läge på en detaljerad nivå är det inte längre möjligt att begränsa en hel organisation (innehavare) till klassiskt läge för listor och bibliotek.

Administratören har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade växlar för att avanmäla dem till följande nivåer:

- webbplats samling
- webbplatsmallar
- förteckning
- Objektbibliotek

Listor som använder vissa funktioner och anpassningar som inte stöds av moderna kommer att fortsätta att automatiskt växla till klassiskt läge.

Med början den 1 april 2019, processen för att inaktivera klient organisations nivå avmarkerar du moderna listor och bibliotek startas och fortsätter genom den 31 maj 2019.  Listor och bibliotek som är i klassiskt läge som ett resultat av att klienter väljer att välja kommer automatiskt att flyttas till moderna.

Om du behöver klassiskt läge kan du läsa mer [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP PowerShell- [instruktioner som](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) beskriver de alternativ och verktyg som du kan använda i dag för att använda klassiskt läge.
