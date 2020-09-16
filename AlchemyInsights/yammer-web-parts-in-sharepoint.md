---
title: Yammer-webbdelar i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664368"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Yammer-webbdelar i SharePoint

Yammer-konversationer och Yammer markerar webb delar förbättrar samarbetet för moderna och klassiska SharePoint-sidor. Mer information finns i [Yammer-konversationer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  och  [Yammer-markeringar](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).    

Webb delen för moderna Yammer-konversationer uppdateras till den nya Yammer-upplevelsen och är tillgänglig för klient organisationer med mål versioner. GA-lanseringen har startat. Med de nya funktionerna kan du starta en konversation med ett inlägg (frågor, omröstningar, beröm) och markera bästa svar direkt från SharePoint. Mer information finns i [nya Yammer-regler och vanliga frågor](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).

 Information om vilken webbdel och konfiguration som passar dig finns i [använda en Yammer-webbdel i SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).  

**Använda webb delar med SharePoint Server**  

Webb delar kan användas på moderna och klassiska sidor i lokala miljöer.

- Mer information om moderna sidor finns i [lägga till en Yammer-feed på en modern sida i SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- Mer information om klassiska sidor finns i [lägga till en Yammer-feed på en klassisk sida i SharePoint server 2013, 2016 och 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Bädda in Yammer**  

Använd verktyget bädda in konfiguration för att testa Inbäddnings användning. En framtida uppdatering av embed aktiverar den nya Yammer-upplevelsen. Mer information finns i [konfigurations verktyget](https://aka.ms/YammerEmbedConfigureTool)för sammanfattning av Yammer. Information om hur du kan förstå komponenten bädda in i Yammer finns i [bädda in feed](https://aka.ms/YammerDevDocs).

**Kända problem och begränsningar**

- Grupp-ID: n är inte tillgängliga från nya Yammer-adresser, som har ändrats. Gå tillbaka till klassiskt läge för att få grupp-ID: n eller andra ID: n från URL: er.
- Anpassade domäner (alternativa) stöds inte.
- Yammer embed är inte optimerat för mobil. Använd moderna sidor med webb delen Yammer-konversationer.
- Anpassade teman kan påverka utseendet och användbarheten hos webb delen Yammer-konversationer. Öppna ett support ärende för att rapportera problem.