---
title: 1491 – sökning-inte returnerar-resultat förväntas
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740492"
---
# <a name="content-search-not-returning-expected-results"></a>Innehålls sökning returnerar inte förväntat resultat

När du kör innehålls sökningar från Microsoft 365 Security & Compliance Center kan du få oväntade Sök resultat. Tänk på följande när du kan påverka Sök resultaten:

- **Innehålls platser och Sök villkor**: kontrol lera att du har valt rätt innehåll och Sök villkor. Om du körde en stor sökning (med många platser) bör du dela upp den i flera sökningar.

- **Delvis indexerade objekt**:  [delvis indexerade objekt](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) från post lådor ingår i det uppskattade Sök resultatet. Delvis indexerade objekt från webbplatser i SharePoint och OneDrive tas emellertid inte med i sökningen.

- **Sök fel**: när du söker i ett stort antal post lådor (över 100 000-postlådor) kan du få Sök fel, med felkoder som CS008-009 och CS012-002). I det här fallet ska du försöka med att söka i sökningen igen. Mer information finns i  [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
