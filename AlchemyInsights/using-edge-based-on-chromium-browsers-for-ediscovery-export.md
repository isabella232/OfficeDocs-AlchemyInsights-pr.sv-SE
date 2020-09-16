---
title: Använda Microsoft Edge baserat på krom webbläsare för eDiscovery-export
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734533"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Använda Microsoft Edge baserat på krom webbläsare för eDiscovery-export

På grund av en senaste ändring har Microsoft Edge-webbläsarna inte längre support för ClickOnce aktiverat som standard. För att kunna fortsätta använda Microsoft 365 eDiscovery export Tool måste du antingen använda Microsoft Internet Explorer eller aktivera ClickOnce support i Microsoft Edge. 

Så här aktiverar du support för ClickOnce i Microsoft Edge baserat på krom: 
1. I webbläsaren Microsoft Edge besöker du edge://flags/#edge-Click-once.
2. För alternativet ClickOnce support ändrar du värdet från **default** eller **Disabled** till **Enabled**. 
3. Välj **starta om**längst ned i webbläsarfönstret. <br>
 Ändringen börjar gälla när du har startat om Microsoft Edge. 

Information om hur du installerar export verktyget finns i: [ Exportera innehålls Sök Resultat](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).