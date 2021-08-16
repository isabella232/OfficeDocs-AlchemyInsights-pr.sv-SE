---
title: Använda Microsoft Edge baserat på Chromium webbläsare för ediscovery-export
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
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998422"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Använda Microsoft Edge baserat på Chromium webbläsare för ediscovery-export

På grund av en ny ändring Microsoft Edge webbläsare inte längre stöd ClickOnce aktiverat som standard. Om du vill fortsätta att använda Microsoft 365 eDiscovery-exportverktyget måste du antingen använda Microsoft Internet Explorer eller aktivera ClickOnce support i Microsoft Edge. 

Så här aktiverar ClickOnce support i Microsoft Edge baserat på Chromium: 
1. Gå till Microsoft Edge i webbläsaren edge://flags/#edge-click-once.
2. För alternativet ClickOnce support ändrar du värdet från Standard **eller** **Inaktiverad** till **Aktiverad.** 
3. Välj Starta om längst ned i **webbläsarfönstret.** <br>
 Ändringen börjar gälla när du startar om Microsoft Edge. 

Mer information om hur du installerar exportverktyget finns i: [ Exportera innehållssökningsresultat](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).