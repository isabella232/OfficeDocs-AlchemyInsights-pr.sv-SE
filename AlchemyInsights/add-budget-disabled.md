---
title: Varför är knappen Lägg till budget inaktive rad för mig?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807671"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Varför är knappen Lägg till budget inaktive rad för mig?

För att skapa en budget behöver du någon av följande behörigheter:

- Hanterings grupp, abonnemang, resurs grupp omfattningar
- Deltagare för kostnads hantering
- Postlådeägare
- Verkar
- Endast företags kund: registrering, avdelning, konto omfattningar
- Registrerings administratör (ange budget vid registrerings omfattning)
- Avdelningens administratör (ange budget på avdelningens omfattning)
- Konto ägare (ange budget för konto omfång)
- Endast moderna kund avtal: fakturerings konto, fakturerings profil, avsnitts omfattningar för faktura
- Azure-prenumeration skapad

**Jag skapade en budget när min kostnad för den aktuella månaden redan hade varit budget. Varför fick jag inte något meddelande?**  
Om du redan har överskridit tröskelvärdet för en viss kostnad när du skapar en budget får aviseringen inte aktive ras. Om du bryter mot tröskeln utlöses varnings meddelandet när en ny cykel påbörjas.

**När ska jag förvänta dig att få en avisering efter att jag har överskridit en av mina definierade tröskelvärden för budget meddelanden?**  
Budgetar utvärderas var fjärde timme. Det tar minst 8 timmar för användnings data att nå budget systemet. På grund av detta kan det ta upp till 12 timmar att utlösa aviseringar efter det att du har överskridit ett tröskelvärde.

**Varför är knappen Start datum inaktive rad när jag väljer en månads-eller fakturerings period?**  
Budgetarna justeras efter den aktuella kalender månaden eller aktuella fakturerings perioden (om fakturerings månad är markerat). Därför fyller vi i det här värdet för dig.

**Varför ser jag inte ett diagram över mina kostnader i budget skapande versionen?**  
Vi behöver minst två månader med kostnads data innan vi kan återge en kurva som hjälper dig att skapa budget.

**Varför kan jag inte ange en budget för en prenumeration som jag just har skapat?**  
När du har skapat ett abonnemang tar informationen 24-48 timmar att bearbeta innan den ställer in en budget för den.

**Budget-API-resurser**

- [Budget API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): tillhandahåller operationer för att skapa och uppdatera budgetar. Med budget-API: t kan du ställa in en budget tröskel och konfigurera flera notifieringar att utlösa när du närmar dig detta. Aviseringar kan utlösa ett e-postmeddelande eller en Azure-åtgärds grupp för att utföra automatisering. Obs! filtrering för detta API justeras inte med API-filtrering för frågor/dimensioner.
- [Budgetar API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): skapa budgetar med högre kostnads filtrerings kapacitet än v1. Filtrering används för att justera kontraktet för frågor och dimensioner. Det här är det rekommenderade budget API: t som används för att flytta framåt.
- [Dimensioner](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): tillhandahåller operationer för att få dimensioner som stöds för användning under en mängd olika omfattningar. Med dimensions-API: t kan du hämta en lista över dimensioner som kan användas som indata för att generera frågor med fråge-API: t.
- [Fråga](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): tillhandahåller operationer för att hämta aggregerade kostnader och användnings data baserat på frågan du tillhandahåller. Med fråge-API: t kan du ange önskat filter, sortering och gruppering för alla tillgängliga dimensioner (som nås från API: t).

**Prognostiserade kostnader**

**Varför ser jag inte prognoser för mina kostnader i kostnads analys?**  
Det finns flera orsaker till varför prognos projektionen kanske saknas för dig i kostnads analys, så här:

1. Om dina kostnads data är mindre än 10 dagar gamla laddas inte prognos diagrammet. Modellen kräver minst 10 dagars senaste kostnads data för korrekt projektion
2. Om du har valt historiskt datum visas inte prognos diagrammet. Välj ett datum intervall med framtida datum för att prognos diagrammet ska visas
3. Om ditt konto har flera valutor kostar prognos diagrammet bara kostnader för "alla kostnader i USD"

**Varför ändras inte prognosen när jag ändrar mina resurser?**  
För prognos modellen krävs ett par dagar för att kontot ska ändras och det gör inga omedelbara projektioner utifrån förändringar i resurser  
För större steg för ökning eller minskning av resurser tar modellen lite längre tid att justera till dessa ändringar för att åtgärda avvikelser

**Varför ökar min prognos när jag har köpt en reservation eller ett Marketplace-inköp?**  
Prognos modellen tar hänsyn till din "faktiska kostnad" och tar inte hänsyn till förbrukning och inköp separat. För en enda köp kan modellen minska projektionerna efter 10 dagar till kontot för den plötsliga ökningen av kostnaderna

**Jag vill visa prognoser för en enda dimension (exempel. Läst**  
Prognosen har stöd för totala kostnads projekt och inte för enskilda mätare. När "grupperas av" en dimension blir projektionerna totalt för alla objekt i dimensionen

**Rekommenderade dokument**

- [Vad är Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Metod tips för Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysera dina kostnader och utgifter](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Utforska och analysera kostnader med kostnads analys](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: priser](https://azure.microsoft.com/services/cost-management/#pricing)
- [Granska kostnader i kostnads analys](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video kurs: skapa en budget i Azure-portalen](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Förutsättningar för att visa och anpassa budgetar](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Skapa och hantera budgetar](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurera Automation med Azure åtgärds grupper och budgetar API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Använd kostnads varningar för att övervaka användning och utgifter](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Metod tips för kostnads hantering](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video kurs**

- [Skapa en budget i Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Hantera kostnader med API och åtgärds grupper i budget](https://go.microsoft.com/fwlink/?linkid=2147038)