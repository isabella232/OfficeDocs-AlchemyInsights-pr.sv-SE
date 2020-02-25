---
title: Active Directory synkroniseras inte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265274"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseras inte

Om du får synkroniseringsfel, till exempel "ingen ny synkronisering" eller märker katalogsynkroniseringsstatus en office-administratörsportal säger: "Senast synkroniserad mer än 3 dagar sedan", kan det hända att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.  

Om du installerar om AADConnect med hjälp av expressinställningar kan problemet lösas snabbt:

1. [Ladda ner den senaste versionen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Följ instruktionerna för expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Mer information om AADConnect-tjänstkonton finns i [Azure AD Connect: Konton och behörigheter](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
