---
title: Arbetsflödes e-post skickas inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049391"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbetsflödes e-post skickas inte för en SharePoint-lista eller bibliotek

1. E-post från arbetsflöden skickas inte till alla användare eller endast till vissa användare, eller så visas felmeddelandet **det går inte att skicka e-postmeddelandet. Kontrollera att e-postmeddelandet har en giltig mottagare**.

    Kontrollera om användaren finns i gruppen **alla personer** behörigheter (användarinformation lista) för webbplatssamlingen.  Exempel på direkt URL:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Om användaren inte finns kontrollerar du att användaren är inloggad på sidan. 
    - Om det är en extern användare, se till att deras inbjudan har accepterats.
    - Om användaren finns i gruppen behörigheter, kontrollera att e-postadressen är korrekt.
    - Om användarnas e-postadress inte anges här, skapa en exempel avisering för användaren som tvingar synkronisering av användarkontot från användarprofiler i SharePoint till den här webbplatssamlingen.
 
2. E-post från arbetsflöden skickas till administratörer för webbplatssamlingen, men inte till andra användare och se felet **http förbjuden till <span>https:</span>//url/_vti_bin/client.XVC.sp.Utilities.Utility.sendemail**.
 

    Se [åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontrollera också att den **begränsad åtkomst användare behörighet låsning läge** webbplatssamling funktionen inte är aktiv.


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


