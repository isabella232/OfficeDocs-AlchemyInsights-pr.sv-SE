---
title: Ändra standarddomänen för Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818018"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Ändra standard-/primärdomän för Yammer

Yammer-URL:en innehåller det aktuella primära domännamnet för Yammer-nätverket. Det här domännamnet överensstämmer kanske inte med det primära domännamnet som angetts i Office 365 eller Azure AD. Det finns skillnader i beteende baserat på antalet anpassade domäner som lagts till i klientorganisationen, och om Yammer är i en konfiguration som stöds (1 klientorganisation: 1 nätverk, eller 1:1). Det finns dokumentation om [Yammer-domäner och Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Den vanligaste orsaken till en felaktig domän är att det finns flera Yammer-nätverk som måste konsolideras. Ett viktigt första steg är att [konsolidera till ett enda nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) med hjälp av verktyget för nätverksmigrering. Slutför det här innan du försöker ange din primära domän.

**Inga anpassade domäner**

För nya klientorganisationer används standarddomänen (t.ex. fabrikam.onmicrosoft.com) från klientorganisationen för Yammer. Den primära domänen anges till yammer.com/fabrikam.onmicrosoft.com.

**En anpassad domän**

Yammer väljer automatiskt den anpassade domänen (t.ex. fabrikam.com) från klientorganisationen som primär domän i Yammer. Den anges till yammer.com/fabrikam.com. Den här ändringen görs av domänens synkroniseringstjänst, och det kan ta upp till 24 timmar innan den träder i kraft.

**Flera anpassade domäner**

Yammer kan ha en primär domän som skiljer sig från standarddomänen för klientorganisationen. Eftersom det finns flera anpassade domäner antar Yammer inte vilken den rätta domänen är av de som är tillgängliga. Du måste öppna ett supportärende för att begära att det primära domännamnet ändras till den primära domän du vill använda.

**Ytterligare felsökningsinformation**

I vissa fall kan domäner ha flyttats mellan klientorganisationer och domänens synkroniseringstjänst har inte kunnat köras. Du kanske stöter på inloggningsproblem och andra problem, utöver en felaktig primär domän. För att lösa det här problemet kan domäner behöva flyttas till rätt nätverk med hjälp av Microsoft Support. Denna situation kräver direkt hjälp och kan ta lite tid att lösa, särskilt om det finns en mycket lång lista med domännamn. Öppna ett supportärende för att få hjälp med att lösa sådana här problem.

När du arbetar med en supportagent kontrollerar de att domäner har verifierats på en klientorganisation under din kontroll. De kan ställa ytterligare verifieringsfrågor om domänerna om de har lagts till i din klientorganisation men inte verifierats av DNS. Se till att domäner verifieras av DNS för att göra processen snabbare.
