---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355895"
---
# <a name="content-search-not-returning-expected-results"></a>Innehåll sökningen inte ger förväntade resultat

När du kör innehållssökning från Office 365 säkerhet & regelefterlevnadscentret hända oväntade resultat. Tänk på följande saker som kan påverka dina sökresultat:

- **Innehållsplatser och sökvillkor**: Kontrollera att du har valt rätt innehållsplatser och sökvillkor. Om du körde en stor sökning (med många platser), bör du överväga att dela upp det i flera sökningar.

- **Delvis indexerade objekt**: [delvis indexerade artiklar](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) från postlådor ingår i uppskattade sökresultaten. Dock ingår delvis indexerade artiklar från webbplatser i SharePoint och OneDrive inte i uppskattningen sökning.

- **Sök fel**: när du söker ett stort antal postlådor (över 100 000 postlådor), kan du få söka fel med felkoder som CS008-009- och CS012-002). Försök i så fall Sök endast efter de misslyckade innehållsplatser. Finns i [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) för mer information.
