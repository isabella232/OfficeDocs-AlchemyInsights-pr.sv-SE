---
title: Blockera nedladdning på delningslänkar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358512"
---
# <a name="block-download-on-sharing-links"></a>Blockera nedladdning på delningslänkar

**Hämtning av block** är tillgängligt för **endast visningslänkar** till Office-dokument. När du väljer det här alternativet visas inte alternativ för att hämta, skriva ut eller kopiera filen när du får åtkomst till filen via länken som du skapade.

Administratörer kan styra om inställningen "blockera hämtning" bara visas för Office-filer eller inte genom att ändra `BlockDownloadLinksFileType` inställningen i [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) eller [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell-cmdlets.
