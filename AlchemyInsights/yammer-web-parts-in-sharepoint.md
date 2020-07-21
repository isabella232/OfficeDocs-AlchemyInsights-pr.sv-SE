---
title: Yammer-webbdelar i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198383"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Yammer-webbdelar i SharePoint

Yammer Conversations och Yammer Highlights-webbdelar förbättrar samarbetet på moderna och klassiska SharePoint-sidor. Mer information finns i [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) och [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).    

Den moderna webbdelen Yammer Conversations uppdateras till den nya Yammer-upplevelsen och är tillgänglig för målgåsresättare. GA-utrullningen har startat. Nya funktioner inkluderar möjligheten att starta en konversation med valfritt inlägg (Frågor, omröstningar, beröm) och att markera de bästa svaren direkt från SharePoint. Mer information finns i [Nya Yammer-kundvillkor och vanliga frågor och svar .](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)

 Information om vilken webbdel och konfiguration som är rätt för dig finns [i Använda en Yammer-webbdel i SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).  

**Använda webbdelar med SharePoint Server**  

Webbdelar kan användas i moderna och klassiska sidor i lokala miljöer.

- Mer information om moderna sidor finns i [Lägga till en Yammer-feed på en modern sida i SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- Mer information om klassiska sidor finns i [Lägga till en Yammer-feed på en klassisk sida i SharePoint Servers 2013, 2016 och 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Yammer Bädda in**  

Använd verktyget Bädda in konfiguration för att testa inbäddningsanvändning. En framtida uppdatering av Bädda in aktiverar den nya Yammer-upplevelsen. Mer information finns i verktyget Konfigurationsverktyg för [Yammer Embed](https://aka.ms/YammerEmbedConfigureTool). Mer om du vill förstå Yammer Embed-komponenten bättre finns [i Bädda in feed](https://aka.ms/YammerDevDocs).

**Kända problem och begränsningar**

- Grupp-ID:er är inte tillgängliga från nya Yammer-URL:er, som har ändrats. Växla tillbaka till klassiskt läge för att hämta grupp-ID:n eller andra ID:n från webbadresser.
- Anpassade (fåfänga) domäner stöds inte.
- Yammer Embed är inte optimerad för mobilen. Använd moderna sidor med webbdelen Yammer Conversations för bästa möjliga upplevelse.
- Anpassade teman kan påverka utseendet och användbarheten av webbdelen Yammer Conversations. Öppna ett supportärende för att rapportera problem.