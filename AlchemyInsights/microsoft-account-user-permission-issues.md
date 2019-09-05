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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754210"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsöka problem-användare hittades inte i katalogen

Om användare får felmeddelandet "användaren kan inte hittas" i katalogen. Försök igen där problemtypen är användare inte i katalogen.

Följande steg kan slutföras för att felsöka problemet.

- Se till att kontot som accepterade e-postinbjudan är samma konto som används för att logga in senare. Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. 

Mer information finns i hantera [alias för ditt Microsoft-konto</a> för att hantera Office 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bläddra till varje plats (er) där användaren får felet. 

Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbla citationstecken) i slutet av webbplatsens URL. 

Exempel: https://_ lt _ "contoso">. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.

- Markera användaren i listan.

- Klicka på **ta bort användarbehörigheter** från menyfliksområdet. 
-  Lägg tillbaka användaren och skicka inbjudan till användaren igen.

