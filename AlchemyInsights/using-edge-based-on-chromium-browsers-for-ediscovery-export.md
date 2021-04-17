---
title: Använda Microsoft Edge baserat på Chromium-webbläsare för Ediscovery-export
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834389"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Använda Microsoft Edge baserat på Chromium-webbläsare för Ediscovery-export

På grund av en ny ändring kommer Microsoft Edge-webbläsare inte längre att ha ClickOnce-stöd aktiverat som standard. Om du vill fortsätta att använda Microsoft 365 eDiscovery-exportverktyget måste du antingen använda Microsoft Internet Explorer eller aktivera ClickOnce-supporten i Microsoft Edge. 

Aktivera ClickOnce-supporten i Microsoft Edge baserat på Chromium: 
1. I webbläsaren Microsoft Edge går du till sidan edge://flags/#edge-click-once.
2. För alternativet ClickOnce Support ändrar du värdet från **Standard eller** **Inaktiverad** till **Aktiverad.** 
3. Välj Starta om längst ned i **webbläsarfönstret.** <br>
 Ändringen börjar gälla när du startat om Microsoft Edge. 

Mer information om hur du installerar exportverktyget finns i: [ Exportera innehållssökningsresultat](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).