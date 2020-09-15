---
title: Teams 4c7-fel
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700221"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 fel i Microsoft Teams

Det här felet beror på att Microsoft Teams kräver formulärautentisering. När du distribuerar AD FS (Active Directory Federation Services) är formulärautentisering inte aktiverat för intranätet som standard. Om Windows-integrerad autentisering inte fungerar uppmanas du att logga in med formulärautentisering.

Lös problemet genom att aktivera formulärautentisering med snapin-modulen AD FS Microsoft Management Console (MMC) på den dator som har den lokala kopian av Active Directory. Gör så här: 

1. Bläddra till **autentiseringsprinciper**i navigerings fönstret.
2. Välj **Redigera global primär verifikation**under **åtgärder** i informations fönstret.
3. Välj **formulärautentisering**på fliken **intranät** .
4. Välj **OK** (eller **Använd**).