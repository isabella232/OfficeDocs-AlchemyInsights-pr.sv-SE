---
title: Felsökning - användare som inte finns i katalogen
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544881"
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

