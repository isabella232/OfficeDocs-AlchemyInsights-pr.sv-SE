---
title: Omfattande SharePoint-listor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720151"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeta med stora listor och bibliotek i SharePoint

SharePoint-listor och-bibliotek kan innehålla upp till 30 000 000 objekt, men när de har mer än 5 000 objekt kanske ett fel meddelande visas när du försöker arbeta med dem. Tröskelvärdet är till för att upprätthålla tjänstens prestanda. Det kan inte ändras. För att undvika att det här tröskelvärdet uppnåddes:

**Använd moderna**

Vyer som visar många objekt fungerar bäst i den moderna upplevelsen. [Använd den moderna upplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) för att undvika fel som kan uppstå i den klassiska upplevelsen.

**Lägga till index**

När du filtrerar eller sorterar efter en kolumn som inte har ett index kanske du får ett fel meddelande. [Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt från **list inställningar** på menyn Inställningar och sedan **indexerade kolumner**.

**Redigera listvyn**

Om det uppstår ett fel när du arbetar med en stor lista [redigerar du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Följande fyra ändringar tar bort tröskelvärden för listvyer. Gör alla fyra ändringar för att ta bort alla fel. Om du fortfarande får fel meddelanden markerar du [hantera stora listor och bibliotek](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Välj **ingen** från **den första sorteringen efter kolumnen** och **Sortera sedan efter kolumnen**.
2. Välj **ingen** från **den första gruppen efter kolumnen** och **Gruppera sedan efter kolumnen**.
3. Välj **ingen** för alla kolumner i avsnittet **summor** .
4. Avmarkera alla **kolumner** utom en i kolumnerna.

