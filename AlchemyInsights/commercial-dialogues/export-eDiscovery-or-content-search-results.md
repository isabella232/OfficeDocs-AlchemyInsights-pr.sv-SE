---
title: Exportera resultat för eDiscovery/innehållssökning
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483736"
---
# <a name="export-ediscoverycontent-search-results"></a>Exportera resultat för eDiscovery/innehållssökning

Du kan behöva exportera sökresultatet till en PST-fil (från e-post) eller till interna Office-dokument (från SharePoint- och OneDrive för företag-webbplatser). Gör i så fall följande:

- Kontrollera att ditt konto har rätt behörighet att exportera. Mer information finns i Tilldela [eDiscovery-behörighet.](https://go.microsoft.com/fwlink/?linkid=2102406)
- Kontrollera att datorn har uppfyllt alla [krav.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Alla webbläsare stöds inte, till exempel Chrome.
- Exportera från en innehållssökning: a. Gå till [Säkerhets- & Center för](https://protection.office.com/contentsearch) efterlevnad, klicka **på** Sök och välj sedan **Innehållssökning.** Välj **en sparad** sökning på sidan Innehållssökning.
    b. Välj Starta export under Exportera **resultat till en** dator i **informationsfönstret.** Om du exporterar fler än 100 000 postlådor måste du använda PowerShell för att ladda ned exportresultaten. Mer information finns i Exportera [resultat från fler än 100 000 postlådor.](https://go.microsoft.com/fwlink/?linkid=2143861)

Mer information finns i [Exportera sökresultat för innehåll.](https://go.microsoft.com/fwlink/?linkid=2102118)