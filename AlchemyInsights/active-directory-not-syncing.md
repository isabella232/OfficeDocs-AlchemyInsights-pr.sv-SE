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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930993"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseras inte

Om du får synkroniseringsfel, till exempel "ingen ny synkronisering", eller om katalogsynkroniseringsstatusen visas i administrationsportalen för Office står det "Senaste synkroniseringen för mer än 3 dagar sedan" kan det vara så att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.  

Om du installerar om AADConnect med standardinställningarna kan problemet snabbt lösas:

1. [Ladda ned den senaste versionen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Följ anvisningarna för expressinstallation](/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect måste installeras på Windows Server 2012 eller senare. Servern måste vara domänansluten och kan vara en domänkontrollant eller en medlemsserver. En fullständig lista över krav och förutsättningar Anslut Azure AD finns i Förutsättningar [för Azure AD Anslut.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Mer information om AADConnect-tjänstkonton finns i [Azure AD Anslut: Konton och behörigheter.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
