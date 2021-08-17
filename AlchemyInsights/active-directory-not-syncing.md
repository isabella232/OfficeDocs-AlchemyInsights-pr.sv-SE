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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889236"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseras inte

Om du får synkroniseringsfel, till exempel "ingen ny synkronisering", eller om katalogsynkroniseringsstatusen visas i administratörsportalen i Office står det "Synkroniserades senast för mer än 3 dagar sedan" kan det vara så att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.  

Om du installerar om AADConnect med standardinställningarna kan problemet snabbt lösas:

1. [Ladda ned den senaste versionen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Följ anvisningarna för expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect måste installeras på Windows Server 2012 eller senare. Servern måste vara domänansluten och kan vara en domänkontrollant eller en medlemsserver. En fullständig lista över krav och förutsättningar Anslut Azure AD finns i Förutsättningar [för Azure AD Anslut.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Mer information om AADConnect-tjänstkonton finns i [Azure AD Anslut: Konton och behörigheter.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
