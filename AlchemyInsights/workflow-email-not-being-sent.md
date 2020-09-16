---
title: E-postmeddelandet skickas inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749027"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-postmeddelandet skickas inte för en SharePoint-lista eller ett bibliotek

1. E-post från arbets flöden skickas inte till alla användare eller bara vissa användare, eller så visas fel **meddelandet. kontrol lera att e-postmeddelandet har en giltig mottagare**.

    Kontrol lera om användaren finns i gruppen **all personal** behörigheter (användar information) för webbplats samlingen.  Exempel direkt adress: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Om användaren inte finns kontrollerar du att användaren är inloggad på sidan. 
    - Om det är en extern användare kontrollerar du att deras inbjudan har accepterats.
    - Om användaren finns i behörighets gruppen kontrollerar du att e-postadressen är korrekt.
    - Om användarnas e-postadress inte är inställt här skapar du ett exempel på en avisering för den användaren som tvingar synkroniseringen av användar kontot från användar profiler i SharePoint till den här webbplats samlingen.
 
2. E-post från arbets flöden skickas till webbplats samlingens administratörer men inte till andra användare och se **http-felet otillåtet för <span>https:</span>//url/_vti_bin/client.XVC.sp.Utilities.Utility.sendemail**.
 

    Se [åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontrol lera också att funktionen för att **nedlåst behörighets läge för användare med begränsad åtkomst** inte är aktiv.


## <a name="related-topics"></a>Relaterade ämnen
Vill du prova Microsoft Flow i SharePoint Online?
- [Skapa flöde](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint och flöde](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


