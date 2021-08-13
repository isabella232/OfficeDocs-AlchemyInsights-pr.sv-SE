---
title: Varför är knappen Lägg till budget inaktiverad för mig?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954709"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Varför är knappen Lägg till budget inaktiverad för mig?

För att skapa en budget behöver du någon av följande behörigheter:

- Hanteringsgrupp, prenumeration, resursgruppomfattningar
- Deltagare i kostnadshantering
- Ägare
- Deltagare
- Endast företagskund: Registrering, Avdelning, Kontoomfattningar
- Registreringsadministratör (ange budget i omfattningen Registrering)
- Avdelningsadministratör (ange budget för avdelningsomfång)
- Kontoägare (ange budget för kontoomfattning)
- Endast moderna kundavtal: Faktureringskonto, Faktureringsprofil, Fakturaavsnittsomfattningar
- Skapa Azure-prenumeration

**Jag skapade en budget när min kostnad för den aktuella månaden redan över budgeterades. Varför fick jag ingen avisering?**  
Om du redan har överskridit ett visst kostnadströskelvärde när du skapar en budget som inte kommer att uppmärksammas. När en ny cykel börjar, och du bryter mot tröskelvärdet, kommer aviseringen att skjutas upp.

**När ska jag förväntar mig att få en avisering när jag överskrider ett av mina definierade tröskelvärden för budgetavisering?**  
Budgetar beräknas var fjärde timme. Det tar minst 8 timmar för användningsdata att nå budgetsystemet. På grund av detta kan det ta upp till 12 timmar innan aviseringar kan skjutas upp till 12 timmar efter att du har överskridit ett tröskelvärde.

**Varför är knappen Startdatum inaktiverad när jag väljer en återställningsperiod för månad eller faktureringsmånad?**  
Budgetar justeras efter den aktuella kalendermånaden eller aktuell faktureringsperiod (i det fall faktureringsmånad är markerad). Därför fyller vi i det här värdet åt dig i förväg.

**Varför visas inget diagram över mina kostnader när jag skapar budget?**  
Vi behöver minst 2 månaders kostnadsdata innan vi kan återge ett diagram som hjälper dig att skapa budget.

**Varför kan jag inte ange en budget för en prenumeration som jag just skapade?**  
När du har skapat en prenumeration tar det 24–48 timmar att bearbeta data innan du anger en budget för den.

**Budget-API-resurser**

- [Budgetar API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Tillhandahåller åtgärder för att skapa och uppdatera budgetar. Med hjälp av budget-API:t kan du ange ett budgettröskelvärde och konfigurera flera aviseringar när du närmar dig tröskelvärdet. Aviseringar kan utlösa ett e-postmeddelande eller en Azure-åtgärdsgrupp för att utföra automation. Obs! Filtrering för detta API justeras inte mot filtrering/mått för Query API.
- [Budget api v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Skapa budgetar med bättre filtreringsfunktioner än v1. Filtreringen justeras efter det kontrakt som används i våra API:er för frågor och dimensioner. Det här är det rekommenderade budget-API:t för att flytta framåt.
- [Dimensioner:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Tillhandahåller åtgärder för att få dimensioner som stöds för din användning under en mängd olika omfattningar. Med Hjälp av Dimensions API kan du hämta en lista med dimensioner som kan användas som indata för att generera frågor med Fråge-API.
- [Fråga:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Tillhandahåller åtgärder för att få aggregerade kostnads- och användningsdata baserat på frågan du anger. Med fråge-API:t kan du ange önskad filtrering, sortering och gruppering för alla tillgängliga dimensioner (som du öppnar via Dimensions API).

**Prognostiserade kostnader**

**Varför ser jag inte prognoser för mina kostnader i Kostnadsanalys?**  
Det finns flera orsaker till att prognosen kan saknas i Kostnadsanalys. Några av dem är följande:

1. Om dina kostnadsdata är mindre än 10 dagar gamla läses inte prognosdiagrammet in. Modellen kräver minst 10 dagar av de senaste kostnadsdata för korrekta projektioner
2. Om du har valt historiska datum kommer prognosdiagrammet inte att visas. Välj ett datumintervall med framtida datum för att prognosdiagrammet ska visas
3. Om ditt konto har flera valutor visas bara projektkostnader för Alla kostnader i USD i prognosdiagrammet

**Varför ändras inte prognosen när jag gör ändringar i mina resurser?**  
Prognosmodellen kräver ett par dagar på sig för ändringar i kontot och några prognoser som inte sker omedelbart utifrån ändringar i resurser  
För större steg om resurser ökar eller minskar tar modellen något längre tid att justera sig efter ändringarna.

**Varför ökar prognosen när jag gör en reservation eller ett marketplace-köp?**  
Prognosmodellen tar hänsyn till din faktiska kostnad och tar inte hänsyn till användning och köp separat. Vid ett köp som bara är ett tillfälle kommer modellen att minska projektionerna efter 10 dagar för att den plötsligt ökade kostnader

**Jag vill se prognoser för en enda dimension (t.ex. Meter)**  
Prognosen har för närvarande stöd för totala kostnadsprognoser och inte för enskilda meter. När en dimension grupperas kommer projektionerna därför att användas för alla objekt i dimensionen

**Rekommenderade dokument**

- [Vad är Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Metodtips för Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysera kostnader och utgifter](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Utforska och analysera kostnader med kostnadsanalys](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Priser](https://azure.microsoft.com/services/cost-management/#pricing)
- [Granska kostnader i kostnadsanalyser](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videokurs: Skapa en budget i Azure Portal](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Förutsättningar för att visa och anpassa budgetar](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Skapa och hantera budgetar](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurera automation med API:t för Azure-åtgärdsgrupper och budgetar](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Använda kostnadsvarningar för att övervaka användning och utgifter](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Metodtips för kostnadshantering](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videokurs**

- [Skapa en budget i Azure Portal](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Hantera kostnader med budget-API och åtgärdsgrupper](https://go.microsoft.com/fwlink/?linkid=2147038)