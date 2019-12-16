---
title: Felsöka problem-användare hittades inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054828"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsöka problem-användare hittades inte i katalogen

Om användare får felmeddelandet "användaren kan inte hittas" i katalogen, vänligen försök igen där problemtypen är användaren inte i katalogen.

Följande steg kan slutföras för att felsöka problemet.

- Se till att kontot som accepterade e-postinbjudan är samma konto som används för att logga in senare. Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. 

Mer information finns i hantera [alias för ditt Microsoft-konto</a> för att hantera Office 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bläddra till varje plats (er) där användaren får felet. 

Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbla citationstecken) i slutet av webbplatsens URL. 

Exempel: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Markera användaren i listan.

- Klicka på **ta bort användarbehörigheter** från menyfliksområdet. 
-  Lägg tillbaka användaren och skicka inbjudan till användaren igen.

