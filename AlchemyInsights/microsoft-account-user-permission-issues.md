---
title: Felsöka problem - Användaren hittades inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702756"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsöka problem - Användaren hittades inte i katalogen

Om användarna får felmeddelandet "användaren kan inte hittas" i katalogen, försök igen där ärendetypen är Användaren inte i katalogen.

Följande steg kan slutföras för att felsöka problemet.

- Kontrollera att kontot som accepterade e-postbjudan är samma konto som används för att logga in senare. Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. 

Mer information finns i [Så här hanterar</a> du alias för ditt Microsoft-konto för att hantera Microsoft 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bläddra till varje webbplats där användaren tar emot felet. 

Lägg till "/_layouts/15/people.aspx/membershipgroupid=0" (inom dubbelcitat) i slutet av webbadressen. 

Exempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Välj användaren i listan.

- Klicka på **Ta bort användarbehörigheter** från menyfliksområdet. 
-  Lägg tillbaka användaren och skicka inbjudan igen till användaren.

