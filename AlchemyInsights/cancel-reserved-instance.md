---
title: Avboka reservering
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819710"
---
# <a name="cancelling-reservation"></a>Avboka reservering

- **Självbetjäning:** Du kan avboka eller byta ut en bokad instans på egen hand med hjälp av [Microsoft Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj en bokning och klicka på återbetalning eller byt ut. Observera att du måste ha ägaråtkomst till bokningsordern för att kunna byta ut den eller få en återbetalning. Endast bokningsåtkomst ger dig inte rätt att fortsätta med din återbetalning eller ombokning. Be bokningsorderns ägare att ge dig ägaråtkomst till bokningsordern
- **Ombokningsprincip:** Du kan byta ut en bokning om du vill boka något annat av samma typ – det finns **inga extra avgifter** för byten. Det totala åtagandet med en ny bokning bör vara större än summan av den utbytta återbetalningen och de framtida månadsbetalningarna (om tillämpligt)
- **Återbetalningsprincip:** Summan av återbetalningen och de avsagda framtida betalningarna får inte överstiga 50 000 USD i en rörlig tidsperiod på 12-månaders. Vi debiterar **för nuvarande inga avgifter** för återbetalningar men kan debitera det för framtida återbetalningar  
    **Undantag:** självbetjäning för ombokningar och avbokningar är inte tillgängligt för kunder som har ett US Government Enterprise Agreement-avtal
- **API/PS/CLI**-support är inte tillgänglig för avbokning och återbetalning [Självbetjäning för ombokningar och återbetalningar för Azure-bokningar](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Självbetjäning för ombokningar och avbokningar är inte tillgängligt för kunder som har ett US Government Enterprise Agreement-avtal. Andra prenumerationstyper för amerikanska myndigheter, till exempel Betala allteftersom och CSP, stöds

Läs mer: [hur retur- och ombokningstransaktioner bearbetas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Läs mer: [omboknings- och återbetalningsprinciper](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andra frågor: [öppna bokade instansdokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Byt ut en befintlig bokad instans (självbetjäning)**

Du kan byta ut en bokning mot en annan bokning av samma typ. Du kan också få en återbetalning för en bokning på upp till 50 000 USD per år om du inte längre behöver den. Självbetjäning för ombokningar och avbokningar är inte tillgängligt för kunder som har ett US Government Enterprise Agreement-avtal. Andra prenumerationstyper för amerikanska myndigheter, till exempel Betala allteftersom och CSP, stöds. Du måste ha ägaråtkomst till bokningsordern för att kunna boka om den eller få en återbetalning för en existerande bokning.

Följande steg guidar dig genom proceduren för att slutföra transaktionen

1. Logga in på din [Azure-portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj de bokningar som du vill få en återbetalning för och klicka på **Byt ut**
2. Markera VM-produkten som du vill köpa och ange antal. Kontrollera att totalsumman för det nya köpet är mer än retursumman [Fastställ rätt storlek innan du köper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Granska och slutför transaktionen

**Återbetalning för en bokad instans**

Om du vill få en återbetalning för en bokning går du till **bokningsinformation** och klickar på **Återbetalning**

**Proportionell återbetalning:**

**Exempel på propertionell och minimikrav för återbetalning och utbyte**  
Exempel på bokning med förskottsbetalning:

- Du köper en ettårig RI-termin för 120 USD den 1 januari
- Den 7 april vill du få pengarna tillbaka eller byta ut denna bokning
- Eftersom bokningen har varit live i 97 dagar får du (1-97/365) * 120 USD tillbaka. (dvs. 88,1 USD). Det finns för närvarande inga avgifter för återbetalningar
- Om du byter ut bokningen ska det nya köpet vara större än 88,1 USD
- Det finns inga avgifter för återbetalningar för närvarande

**Exempel på bokning med faktureringsplan:**

- Du köper en ettårig RI-termin för 10 USD den 1 januari
- Den 7 april vill du få pengarna tillbaka eller byta ut denna bokning
- Eftersom den senaste betalningen skedde för 7 dagar sedan får du (1-7/31)* 10 USD tillbaka. (dvs. 7,74 USD).
- De avsagda framtida betalningarna ligger på 80 USD. Det finns för närvarande inga avgifter för återbetalningar
- Den här avbokningen drar 87,74 USD från återbetalningsgränsen på 50 000 USD
- Om du byter ut ska det nya köpet vara större än 87,74 USD

**Rekommenderade dokument**

- [Hur retur- och ombokningstransaktioner bearbetas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Omboknings- och återbetalningsprinciper](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)