---
title: Arbetsflödesmeddelande skickas inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766151"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbetsflödesmeddelande skickas inte för en SharePoint-lista eller ett SharePoint-bibliotek

1. E-post från arbetsflöden skickas inte till alla användare eller bara specifika användare, eller så visas felet **E-postmeddelandet kan inte skickas. Kontrollera att e-postmeddelandet har en giltig mottagare**.

    Kontrollera om användaren finns i gruppen **Behörigheter för alla personer** (användarinformationslista) för webbplatssamlingen.  Exempel på direkt webbadress:<tenant>https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0

    - Om användaren inte finns kontrollerar du att användaren är inloggad på sidan. 
    - Om det är en extern användare kontrollerar du att inbjudan har accepterats.
    - Om användaren finns i behörighetsgruppen kontrollerar du att e-postadressen är korrekt.
    - Om användarens e-postadress inte anges här skapar du en exempelavisering för den användaren som tvingar synkroniseringen av användarkontot från Användarprofiler för SharePoint till den här webbplatssamlingen.
 
2. E-post från arbetsflöden skickas till administratörerna för webbplatssamlingen men inte till andra användare och visas felet **HTTP Forbidden till <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontrollera också att webbplatsinsamlingsfunktionen för **användarbehörighetslåsningsläge** för begränsad åtkomst inte är aktiv.


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


