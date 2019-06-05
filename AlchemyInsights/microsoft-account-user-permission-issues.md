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
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717364"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Felsökning - användare som inte finns i katalogen

<p>Om användare får felmeddelandet <strong> &ldquo; &hellip;kan&rsquo;t hittas i katalogen. Försök igen&hellip; </strong> där den typ av problem är <strong> &ldquo;användare inte i katalogen.&rdquo;</strong>, följande åtgärder kan utföras för felsökning av problemet.</p> <ol> <li>Se till att det konto som har accepterat postinbjudan e-är samma konto som används för att logga in senare. Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen. <br /><br />Mer information finns i <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">hur du hanterar alias för ditt Microsoft-konto</a> för att hantera Office 365-inloggning. <br /><br /></li> <li>Bläddra till varje plats där användaren får felet. <br /><br />en. Lägg till <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (inom citattecken) i slutet av webbplatsens URL. <br /><br />Exempel: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Markera användaren i listan. <br /><br />c. Klicka på <strong>Ta bort användarbehörigheter från menyfliken</strong>. <br /><br />d. Lägg tillbaka till användaren och skicka inbjudan till användaren.</li> </ol>

