---
title: Active Directory synkroniserar inte
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697647"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniserar inte

Om du får synkroniseringsfel, till exempel "ingen senaste synkronisering" eller Observera att status för katalog synkroniseringen i administrations portalen för Office visar "senast synkroniserat för mer än 3 dagar sedan", kan det bero på att AADConnect har felaktiga inställningar eller otillräcklig behörighet att utföra en synkronisering.  

Det kan lösa problemet snabbt genom att installera om AADConnect med hjälp av snabb inställningar:

1. [Ladda ner den senaste versionen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Följ anvisningarna för snabb installationen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Mer information om AADConnect-tjänst konton finns i [Azure AD Connect: accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
