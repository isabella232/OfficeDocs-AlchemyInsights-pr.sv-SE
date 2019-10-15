---
title: SharePoint stora listor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488535"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeta med stora listor och bibliotek i SharePoint

SharePoint-listor och-bibliotek kan innehålla upp till 30 000 000 objekt, men när de har fler än 5 000 objekt kan du se ett tröskelvärde för listvy-fel när du försöker arbeta med dem. Det här tröskelvärdet är på plats för att upprätthålla tjänstens prestanda. Det går inte att ändra. Så här undviker du att träffa denna tröskel:

**Använda moderna**

Vyer som visar många objekt fungerar bäst i den moderna upplevelsen. [Använd den moderna upplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) för att undvika fel som du kan se i den klassiska upplevelsen.

**Lägg till index**

När du filtrerar eller sorterar efter en kolumn som inte har ett index kan ett felmeddelande visas. [Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt från **list inställningar** på menyn Inställningar och sedan **indexerade kolumner**.

**Redigera listvyn**

Om ett fel uppstår när du arbetar med en stor lista [redigerar du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Följande fyra ändringar tar bort fel i listvyns tröskelvärde. Gör alla fyra ändringarna för att ta bort alla fel. Om du fortfarande får fel, kontrollera [hantera stora listor och bibliotek](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Välj **ingen** från båda **först sortera efter kolumnen** och **Sortera sedan efter kolumnen**.
2. Välj **ingen** från **den första gruppen i kolumnen** och **Gruppera sedan efter kolumnen**.
3. Välj **ingen** för alla kolumner i avsnittet **summor** .
4. Avmarkera alla utom en kolumn för visning från avsnittet **kolumner** .

