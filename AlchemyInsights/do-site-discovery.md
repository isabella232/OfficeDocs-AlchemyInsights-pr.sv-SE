---
title: Göra webbplatsidentifiering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694556"
---
# <a name="do-site-discovery"></a>Göra webbplatsidentifiering

Om din organisation fortfarande använder äldre webbprogram och planerar att använda Internet Explorer-läge (vilket de flesta kunder gör) bör du göra ytterligare webbplatsidentifiering.

**Du har redan distribuerat en äldre version av Microsoft Edge**

Om du redan har konfigurerat din företagswebbplatslista så att den fungerar för den äldre versionen av Microsoft Edge är webbplatsidentifieringen nästan klar. Det enda du kan behöva göra är att lägga till neutrala webbplatser.

Neutrala webbplatser är vanligtvis webbplatser som tillhandahåller enkel inloggning (SSO). Om du går till en neutral webbplats från Microsoft Edge vill du vara kvar i Microsoft Edge för att autentisera. Om du går till en neutral webbplats i Internet Explorer-läge vill du fortsätta att autentisera i Internet Explorer-läge.

Identifiera SSO-webbplatser eller andra neutrala webbplatser som du använder och lägg till dem i din lista över företagswebbplatser.

**Internet Explorer är din standardwebbläsare**

Om du bara använder Internet Explorer nu kanske du inte vet vilka webbplatser som har uppgraderat till moderna webbstandarder och vilka som fortfarande kräver Internet Explorer. Du vill söka efter och lägga till webbplatserna i listan över företagswebbplatser så att du endast kan använda Internet Explorer-läget för de webbplatserna.

> [!NOTE]
> [Identifiering av företagswebbplats](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) identifierar webbplatser som kan behöva Internet Explorer-läge. Den kan samla in data på datorer med Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.

**Analysera data**

När du har samlat in webbplatsdata rekommenderar vi följande fyrastegsprocess för att analysera data:
1. Sortera data efter domän och sedan efter URL.
2. Definiera gränserna för ett program för att konfigurera för Internet Explorer-läge. Du vill ta med alla webbplatser och webbkontroller som definierar programmet, men du vill inte ta med extra webbplatser och kontroller. Vissa webbplatser kan vara lika enkla som *https://contoso.com/app1* medan andra kan kräva att du definierar flera webbplatser och sidor.
3. Testa programmet för att verifiera att det inte fungerar inbyggt. Många webbplatser erbjuder modernt innehåll när de identifierar en modern webbläsare och erbjuder endast äldre innehåll när de upptäcker Internet Explorer.
4. Lägg till programmet i företagswebbplatslistan om det inte går att testa.

> [!NOTE]
> En god metod är att gruppera alla webbplatser som en app består av. På så sätt är det enklare att ta bort hela webbplatsen från Internet Explorer-läget när du uppgraderar en app och börja använda en modern webbläsare för appen.

När du är klar med webbplatsupptäckten och analyserat data är du redo att börja titta på din kanalstrategi.

