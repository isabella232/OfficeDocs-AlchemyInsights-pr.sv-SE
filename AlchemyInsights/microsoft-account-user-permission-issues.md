---
title: Skapa och använda en delad postlåda
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762418"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsökning - användare som inte finns i katalogen

Om användarna får fel meddelande ”användaren kan inte hittas” i katalogen. Försök igen om den typ av fråga användaren inte är i katalogen.

Följande åtgärder kan utföras för felsökning av problemet.

- Se till att det konto som har accepterat postinbjudan e-är samma konto som används för att logga in senare. Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. 

Mer information finns i [hur du hanterar alias för ditt Microsoft-konto</a> att hantera Office 365-inloggning](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bläddra till varje plats där användaren får felet. 

Lägga till ”/ _layouts/15/people.aspx/membershipgroupid=0” (inom citattecken) i slutet av webbplatsens URL. 

Exempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Markera användaren i listan.

- Klicka på **Ta bort användarbehörigheter** från menyfliken. 
-  Lägg tillbaka till användaren och skicka inbjudan till användaren.

