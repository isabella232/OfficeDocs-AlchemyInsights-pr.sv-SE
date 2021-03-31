---
title: 126 Det går inte att hitta ett fel när du får en postlåda i OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426680"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Visas ingen postlåda i Outlook på webben?

Om du använder Outlook på webben och  du får en postlåda som inte kunde hittas på grund av felet har det konto som du använde för att ansluta till Outlook på webben inte någon Exchange Online-licens och därför är ingen postlåda kopplad till kontot. Administratören kan tilldela kontot en licens så här:

1. Öppna [administrationscentret för Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) gå  till Aktiva användare **under** avsnittet Användare och välj den användare som ser felet.

2. På den användarsida som öppnas  går du till avsnittet  Licenser och appar, väljer rätt Platsvärde och tilldelar en licens som innehåller Exchange Online (expandera licensen om du vill se dess information). När du är klar klickar du på **Spara ändringar**.

I vissa fall, om licensen redan har tilldelats ett användarkonto, kan du lösa problemet och få den korrekt etablerad i systemet genom att ta bort och omtilldela licensen: 

- Kontrollera om dina M365 Exchange Online-prenumerationer (och andra, om du har några) är aktuella och inte nyligen har upphört att gälla.

När du har försäkrat dig om att prenumerationen inte har gått ut och en giltig licens har tilldelats användarkontot kan det ta upp till 24 timmar innan licensen etableras, så du kan behöva vänta på att problemet löses. Mer information finns i [Tilldela och hantera licenser.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)