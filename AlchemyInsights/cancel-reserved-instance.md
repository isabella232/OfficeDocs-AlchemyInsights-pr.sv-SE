---
title: Avbryter reservation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807988"
---
# <a name="cancelling-reservation"></a>Avbryter reservation

- **Själv service:** Du kan annullera eller byta ut en reserverad instans med [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj reservation och klicka på åter betalning eller utbyte. Observera att du måste ha ägar åtkomst på reservations ordern till Exchange eller åter betalning. Till gång till reservationen gör inte att du kan fortsätta med åter betalning eller utbytet. Be reservations order ägaren ge dig ägar åtkomst till reservations ordern
- **Exchange-princip:** Du kan utbyta en reservation för en annan reservation av samma typ – det finns **inga sanktioner** för reservation Exchange. Det totala åtagandet med ny reservation ska vara större än summan av den utbytta reservationens åter betalning och framtida månads betalningar (om tillämpligt)
- **Åter betalnings policy:** Summan av åter betalning och de annullerade framtida betalningarna får inte överstiga $50 000 USD i ett rullande fönster med 12 månader. Vi **debiterar för närvarande inte något straff** för åter betalningar men kan debitera det på framtida åter betalningar  
    **Undantag:** Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA:
- Stöd för **API/PS/CLI** är inte tillgängligt för [självbetjänings utbyte och åter betalningar för Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA: Andra amerikanska abonnemangs typer, inklusive betala allt eftersom-CSP stöds

Läs mer: [så här fungerar retur-och växelkurs transaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Läs mer: [policy för utbyte och åter betalning](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andra frågor: [besök reserverade instans dokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange en befintlig reserverad instans (själv tjänst)**

Du kan utbyta en reservation för en annan reservation av samma typ. Du kan också återbetala en reservation, upp till $50 000 USD per år, om du inte längre behöver den. Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA: Andra amerikanska abonnemangs typer, inklusive betala allt eftersom-CSP stöds. Du måste ha ägar åtkomst till reservations ordern för att kunna utbyta eller återbetala en befintlig reservation.

Följ stegen nedan för att slutföra transaktionen

1. Logga in på din [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj de reservationer som du vill återbetala och klicka på **Exchange**
2. Välj den VM-produkt som du vill köpa och ange en kvantitet. Se till att den nya inköps summan är mer än den totala total summan [bestämmer rätt storlek innan du köper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Granska och slutföra transaktionen

**Åter betalning för en reserverad instans**

Om du vill återbetala en reservation går du till **reservations uppgifter** och klickar på **åter betalning**

**Pro-betygsatt åter betalning:**

**Exempel på tekniker och minsta krav för åter betalning och utbyte**  
Exempel på direkt reservation:

- Du köper ett års perioden RI för $120 den 1 januari
- Den sjunde april du vill återbetala eller utväxla denna reservation
- Eftersom reservationen har varit aktiv i 97 dagar får du (1-97/365) * $120 tillbaka. (d.v.s. $88,1). Det finns inga straff för åter betalningar
- Om du utbyter är ditt nya inköp större än $88,1
- Det är för närvarande inga straff för åter betalningar

**Exempel på fakturerings plan reservation:**

- Du köper ett års perioden RI för $10 per månad
- Den sjunde april du vill återbetala eller utväxla denna reservation
- Eftersom den senaste betalningen skedde 7 dagar får du (1-7/31) * $10 tillbaka. (d.v.s. $7,74)
- De framtida betalningarna annulleras $80. Det finns inga straff för åter betalningar
- Denna annullering dras $87,74 från dig att du använder gränsen för $50 000-bidrag
- Om du utbyter bör det totala värdet för nya inköp vara högre än $87,74

**Rekommenderade dokument**

- [Så här behandlas retur-och växelkurs transaktioner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Principer för Exchange och åter betalning](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)