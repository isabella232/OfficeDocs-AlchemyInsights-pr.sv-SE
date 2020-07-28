---
title: Ta bort en privat teams-kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439913"
---
# <a name="delete-a-teams-private-channel"></a>Ta bort en privat teams-kanal

Microsoft är medvetet om ett problem med att ta bort en privat Teams-kanal om du har aktiverat SharePoint-bevarandeprinciper för den underliggande SharePoint-webbplatsen. Microsoft arbetar på en fix. Under tiden kan du använda följande lösningar för att ta bort den privata kanalen.

**Uteslut grupp-/webbplatssamlingen från principen för lagring av Sharepoint.**

1. Gå till administrationsportalen för Office 365 och välj **Visa alla** i det vänstra navigeringsfönstret.
2. Under **Administrationscenter**går du till **Säkerhet & policy för**att förhindra  >  **efterlevnadsdataförlust**  >  **Policy**.
3. Identifiera alla policyer som gäller för Sharepoint-webbplatser och ändra principen så att Sharepoint-webbplatsen för teamet som innehåller den privata kanalen INTE inkluderas i bevarandeprincipen.
4. Spara principen.
    Det kan ta upp till 24 timmar innan principinställningarna börjar gälla.
    När webbplatsen har uteslutits kan du ta bort den privata kanalen.  
    
Du ***kanske kan*** ta bort den privata kanalen med hjälp av Microsoft Teams på din Android-enhet. 

Relaterad SharePoint-information finns [i Det går inte att ta bort objekt i SharePoint Online eller OneDrive för företag](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).