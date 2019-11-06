---
title: 2609-bevarande-eller-eDiscovery-håll
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994100"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Det går inte att ta bort objekt i SharePoint Online eller OneDrive för företag

Du eller dina användare kan inte ta bort objekt i SharePoint Online eller OneDrive för företag eftersom en bevarandeprincip, bevarande etikett eller e-informationsavslöjande håller tillämpas på en SharePoint-webbplats för OneDrive eller ett visst objekt. Detta inkluderar att det inte går att ta bort ett dokument, en dokumentversion, en mapp, ett dokumentbibliotek, en lista, en app, en webbplats eller en webbplatssamling. Här är några exempel på felmeddelanden som kan tas emot om du försöker ta bort ett objekt som behålls:

- "Den här webbplatsen kan inte tas bort eftersom den ingår i en e-informationsavslöjande spärr eller bevarandeprincip"
- "Den här webbplatsen har en efterlevnadsprincip inställd på att blockera borttagning"
- "En efterlevnadsprincip blockerar för närvarande den här webbplats borttagningen"
- "Den här webbplatssamlingen kan inte tas bort eftersom den innehåller webbplatser som ingår i en e-informationsavslöjande spärr eller bevarandeprincip"
- "Du måste ta bort alla objekt i den här mappen innan du tar bort mappen"
- "Versioner av det här objektet kan inte tas bort eftersom den är spärrad eller bevarandeprincip"
- "Objektet kan inte raderas när det är spärrad"
- "Etiketten som används för det här objektet förhindrar att redigeras eller tas bort"
- "Listan kan inte tas bort när spärrad eller bevarandeprincip"
- "Listan kan inte tas bort om den är blockerad eller om en bevarandeprincip tillämpas på den"

Om du vill ta bort objekt i något av dessa scenarier måste bevarandeprincip, bevarande etikett eller e-informationsavslöjande hålla tas bort (eller en webbplats måste undantas från en bevarandeprincip). Du måste antingen inaktivera eller utesluta respektive spärr som orsakar problemet. När en bevarandeprincip eller spärr tas bort kan det ta upp till 24 timmar innan ändringen träder i kraft. 

Information om de olika bevarande-och spärrfunktioner som kan tillämpas på SharePoint-webbplatser och OneDrive-konton finns i något av följande avsnitt.

- [Översikt över bevarandeprinciper](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Översikt över bevarande etiketter](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Hantera spärrar i Avancerad eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery innehar](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Policyer för äldre webbplats stängning och borttagning](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
