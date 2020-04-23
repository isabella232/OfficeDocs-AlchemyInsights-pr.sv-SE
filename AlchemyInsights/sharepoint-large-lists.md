---
title: Stora SharePoint-listor
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767303"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeta med stora listor och bibliotek i SharePoint

SharePoint-listor och -bibliotek kan innehålla upp till 30 miljoner objekt, men när de har fler än 5 000 objekt kan ett tröskelvärde för listvy visas när du försöker arbeta med dem. Tröskelvärdet är till för att upprätthålla tjänstens prestanda. Det kan inte ändras. Så här undviker du att nå denna tröskel:

**Använd moderna**

Vyer som visar många objekt fungerar bäst i den moderna upplevelsen. [Använd den moderna upplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) för att undvika fel som du kan se i den klassiska upplevelsen.

**Lägga till index**

När du filtrerar eller sorterar efter en kolumn som inte har något index kan du se ett felmeddelande. [Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt från **Listinställningar på** inställningsmenyn och sedan **Indexerade kolumner**.

**Redigera listvyn**

Om ett fel uppstår när du arbetar med en stor lista [redigerar du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Följande fyra ändringar tar bort tröskelfel i listvyn. Gör alla fyra ändringarna för att ta bort alla fel. Om du fortfarande får fel kontrollerar du [Hantera stora listor och bibliotek](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Välj **Ingen** från båda **Först sortera efter kolumnen** och sortera sedan efter **kolumnen**.
2. Välj **Ingen** från både **Första gruppen efter kolumnen** och **gruppera sedan efter kolumnen**.
3. Välj **Ingen** för alla kolumner i avsnittet **Summor.**
4. Avmarkera alla utom en kolumn för visning från avsnittet **Kolumner.**

