---
title: Active Directory synkroniseras inte
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822869"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseras inte

Om du får synkroniseringsfel, till exempel "ingen ny synkronisering", eller om katalogsynkroniseringsstatusen visas i Office-administratörsportalen "Synkroniserades senast för mer än 3 dagar sedan" kan det vara så att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.  

Om du installerar om AADConnect med hjälp av standardinställningarna kan problemet snabbt lösas:

1. [Ladda ned den senaste versionen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Följ anvisningarna för expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Mer information om AADConnect-tjänstkonton finns i [Azure AD Connect: Konton och behörigheter.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
