---
title: Felsöka problem-användare hittades inte i katalogen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768819"
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

