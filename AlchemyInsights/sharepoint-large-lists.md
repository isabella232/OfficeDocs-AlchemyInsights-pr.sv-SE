---
title: SharePoint stora listor
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
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941638"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeta med stora listor och bibliotek i SharePoint

SharePoint listor och bibliotek kan innehålla upp till 30 miljoner objekt, men när de har fler än 5 000 objekt kan du få ett fel för tröskelvärde för listvy när du försöker arbeta med dem. Tröskelvärdet är till för att upprätthålla tjänstens prestanda. Det kan inte ändras. Så här undviker du att nå tröskelvärdet:

**Använd modern**

Vyer som visar många objekt fungerar bäst i det moderna programmet. [Använd den moderna versionen för](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) att undvika fel som kan visas i det klassiska programmet.

**Lägga till index**

När du filtrerar eller sorterar efter en kolumn som inte har ett index kan du få ett felmeddelande. [Lägg till ett index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuellt **från Inställningar** i inställningsmenyn och sedan **Indexerade kolumner.**

**Redigera listvyn**

Om det uppstår ett fel när du arbetar med en stor lista redigerar [du listvyn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

De följande fyra ändringarna tar bort tröskelvärdesfel för listvyn. Gör alla fyra ändringar för att ta bort alla fel. Om du fortfarande får felmeddelanden markerar du Hantera [stora listor och bibliotek.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Välj **Ingen** från **både Sortera först efter kolumnen** och Sortera sedan efter **kolumnen**.
2. Välj **Ingen** i **både den första gruppen efter kolumnen** och Sedan gruppera efter **kolumnen**.
3. Välj **Ingen** för alla kolumner i **avsnittet Summor.**
4. Avmarkera alla kolumner utom en för visning i **avsnittet** Kolumner.

