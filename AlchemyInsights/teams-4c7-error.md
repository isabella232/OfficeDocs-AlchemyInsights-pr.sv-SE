---
title: Lag 4c7 fel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796408"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fel i Microsoft Teams

Det här felet beror på att Microsoft Teams kräver formulärautentisering. När du distribuerar Active Directory Federation Services (AD FS) är formulärautentisering inte aktiverat för intranätet som standard. Om Windows-integrerad autentisering misslyckas uppmanas du att logga in med formulärautentisering.

Lös problemet genom att aktivera formulärautentisering med hjälp av snapin-modulen AD FS Microsoft Management Console (MMC) på den dator som har den lokala kopian av Active Directory. Gör så här: 

1. I navigeringsfönstret bläddrar du till **autentiseringsprinciper**.
2. Välj **Redigera global primär autentisering**under **åtgärder** i informationsfönstret.
3. Välj **formulärautentisering**på fliken **intranät** .
4. Välj **OK** (eller **Verkställ**).