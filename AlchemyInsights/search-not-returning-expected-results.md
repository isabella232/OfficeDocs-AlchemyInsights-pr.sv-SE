---
title: 1491-sök-ej-returnera-förväntade-resultat
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709245"
---
# <a name="content-search-not-returning-expected-results"></a>Innehållssökning returnerar inte förväntade resultat

När du kör Innehållssökningar från Microsoft 365-säkerhetstjänsten & Compliance Center kan du få oväntade sökresultat. Tänk på följande saker som kan påverka sökresultaten:

- **Innehållsplatser och sökvillkor**: Kontrollera att du har valt rätt innehållsplatser och sökvillkor. Om du har gjort en stor sökning (med många platser) kan du dela upp den i flera sökningar.

- **Delvis indexerade objekt**: [Delvis indexerade objekt](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) från postlådor ingår i de uppskattade sökresultaten. Delvis indexerade objekt från webbplatser i SharePoint och OneDrive ingår dock inte i sökninguppskattningen.

- **Sökfel**: När du söker i ett stort antal postlådor (över 100 000 postlådor) kan du få sökfel med felkoder som CS008-009 och CS012-002). Försök i det här fallet bara söka efter de misslyckade innehållsplatserna. Se [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) för mer information.
