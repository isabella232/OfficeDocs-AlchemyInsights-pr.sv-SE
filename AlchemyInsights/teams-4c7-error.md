---
title: Teams 4c7-fel
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786687"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fel i Microsoft Teams

Det här felet inträffar eftersom Microsoft Teams kräver autentisering med formulär. När du distribuerar AD FS (Active Directory Federation Services) aktiveras inte formulärautentisering för intranätet som standard. Om Windows-integrerad autentisering inte fungerar uppmanas du att logga in med formsautentisering.

Lös problemet genom att aktivera formulärautentisering med hjälp av SNAPIN-modulen AD FS Microsoft Management Console (MMC) på datorn med den lokala kopian av Active Directory. Gör så här: 

1. Bläddra till Autentiseringsprinciper i **navigeringsfönstret.**
2. Under **Åtgärder** i informationsfönstret väljer du **Redigera global primär autentisering**.
3. På fliken **Intranät** väljer du Autentisering **med formulär**.
4. Välj **OK** (eller **Använd**).