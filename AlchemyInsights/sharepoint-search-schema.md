---
title: Hantera sökschemat i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770569"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>Hantera sökschemat i SharePoint Online

Sök schema styr vad användarna kan söka efter, hur användarna kan söka i det och hur du kan presentera resultaten på dina Sök webbplatser. 

Se [Hantera sökschemat i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) för att få reda på hur du: 
- Ändra sökschemat.
- Skapa hanterade egenskaper.
- Mappa crawlade kart egenskaper till hanterade egenskaper.

Tänk på följande när du hanterar sökschemat:

- Om du får en varning om att **programmet har pausats** när du gör en schema ändring är det här bara tillfällig eftersom det finns tjänst underhåll. 

    Om det finns mer än 24 timmar och du fortfarande upplever varningen kan du logga in ett support ärende.
- När du ändrar hanterade egenskaper eller lägger till nya träder ändringarna i kraft först efter att innehållet har crawlats på nytt. I SharePoint Online sker crawlningen automatiskt baserat på det definierade synkroniseringsschemat.
- Om du vill vara säker på att dina ändringar är crawlade kan du [begära en Omindexering av listan eller biblioteket](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) 

En fullständig översikt över sökschemat finns i [Introduktion till sökschemat](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) 


