---
title: Arbetsflöde för e-post skickas inte
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270690"
---
# <a name="workflow-email-is-not-being-sent"></a>Arbetsflöde för e-post skickas inte

1. Skickas inte e-post från arbetsflöden för alla användare eller bara vissa användare, eller om du ser felet **e-postmeddelandet inte kan skickas. Kontrollera att e-postmeddelandet har en giltig mottagare**.

    Kontrollera om användaren finns i **Alla** behörigheter gruppen (listan med användarinformation) för webbplatssamlingen.  Exempel på direkt URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Om användaren inte finns, kontrollera att användaren har loggat in på sidan. 
    - Om det är en extern användare kontrollerar du att deras inbjudan har accepterats.
    - Om användaren finns i gruppen behörigheter kontrollera e-postadressen är korrekt.
    - Om användare e-postadress har angetts här, skapar du aviseringen för användaren vilket tvingar synkronisering av användarkontot från profiler av SharePoint för den här webbplatssamlingen.
 
2. E-post från arbetsflöden skickas till webbplatssamlingens administratörer men inte till andra användare och se felet **http-förbjudet att <spam> <spam> ** <spam> <spam>.
 

    Se [Åtkomst nekad när du skickat e-brev till grupper](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Kontrollera också att **begränsad åtkomst användarläge behörighet låsning** webbplatssamling funktionen inte är aktiv.


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


