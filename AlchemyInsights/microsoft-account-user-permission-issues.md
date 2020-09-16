---
title: Felsöka problem – användare finns inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725425"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsöka problem – användare finns inte i katalogen

Om det visas ett fel meddelande om att det inte går att hitta användaren i katalogen, försök igen där ärende typen inte finns i katalogen.

Följ de här anvisningarna för att felsöka problemet.

- Kontrol lera att kontot som godkände e-postinbjudanen är samma konto som används för att logga in senare. Kontrol lera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. 

Mer information finns i [hur du hanterar alias för ditt Microsoft-konto </a> för att hantera Microsoft 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bläddra till varje webbplats som användaren får felet från. 

Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbel citat tecken) i slutet av webbplats-URL: en. 

Exempel: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Välj användaren i listan.

- Klicka på **ta bort användar behörigheter** från menyfliksområdet. 
-  Lägg till användaren tillbaka och skicka inbjudan till användaren igen.

