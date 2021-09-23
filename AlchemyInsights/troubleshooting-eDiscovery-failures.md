---
title: 1490-troubleshooting-eDiscovery-failures
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: b60cfc298ee05375523e3660f407ab03e630c861
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481823"
---
# <a name="troubleshoot-content-search-errors"></a>Felsöka fel i Innehållssökning

Har du problem med innehållssökning eller får problem när du exporterar sökresultat?
Får du till exempel följande när du kör sökningar?

- CS007-, CS008- eller CS012-fel

- Fel vid serverns upptagen/timeout

- Programfel inträffade

Eller får du exportfel när du söker i eller exporterar resultat från ett stort antal (fler än 100 000) postlådor?

För de här felen försöker du igen söka efter innehållsplatser som har misslyckats eller uppdatera sökningen genom att minska sökfrågans komplexitet. Till exempel kan en sökning med jokertecken returnera för många resultat för att systemet ska kunna bearbetas, vilket orsakar ett CS007-fel.   

Mer information finns i [Försök att söka](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) efter innehåll igen för att lösa ett fel på en innehållsplats eller Undersöka, felsöka och lösa vanliga [eDiscovery-problem.](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)

Om du exporterar fler än 100 000 postlådor måste du ladda ned exportresultatet. Mer information finns i [Exportera sökresultat för innehåll.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)
