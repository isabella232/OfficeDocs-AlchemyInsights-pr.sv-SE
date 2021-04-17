---
title: Fakturering för reserverat köp av instans
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
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820340"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering för reserverat köp av instans

Det reserverade instansköpet debiteras mot den betalningsmetod som är kopplad till prenumerationen som du väljer vid köpet. Prenumerationstypen måste vara ett enterprise-avtal (erbjudandenummer: MS-AZR-0017P), Pay-As-You-Go (erbjudandenummer: MS-AZR-0003P), Microsofts kundavtal eller CSP.

- För en företagsprenumeration dras debiteringarna av från registreringens monetära åtagandesaldo eller debiteras som övervärde
- För prenumeration med betalning per abonnemang debiteras debiteringarna till kreditkorts- eller fakturabetalningsmetoden för prenumerationen

**Annullera reservation**

- **Självbetjäning:** Du kan avbryta eller byta ut en reserverad instans själv med [hjälp av Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Välj reservationen och klicka på återbetalning eller byte. Observera att du måste ha ägaråtkomst på reservationsbeställningen för att kunna byta eller återbetala. Endast åtkomst till reservationen låter dig inte fortsätta med återbetalning eller byte. Be ägaren av reservationsbeställningen att ge dig ägaråtkomst till reservationsbeställningen
- **Exchange-policy:** Du kan utväxta en reservation för en annan reservation av samma typ – **det finns** inga garantier för bokningsbyte. Det totala åtagandet med nya reservationer bör vara större än summan av den utbytna reservationens återbetalningsbelopp och kommande månadsbetalningar (om tillämpligt)
- **Återbetalningspolicy:** Summan av återbetalningen och de inställda framtida betalningarna får inte överstiga 500 000 USD i ett rullande fönster på 12 månader. Vi **debiterar för närvarande inte några återbetalningar** men kan debitera det vid framtida återbetalningar

**Undantag:** Självbetjäning för byte och avbokning är inte tillgängligt för kunder med ett företagsavtal för amerikanska myndigheter

- **API-/PS-/CLI-support** är inte tillgänglig för avbokning och återbetalning av [börser via självbetjäning](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) och återbetalning för Azure-bokningar
- Funktionen för självbetjäning för byte och avbokning är inte tillgänglig för kunder med amerikanska government Enterprise Agreement. Andra prenumerationstyper för myndigheter i USA, bland annat Betala efter du-går och CSP stöds

Läs mer: [Hur retur- och exchangetransaktioner behandlas Läs mer:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Principer för [Exchange och återbetalning](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Andra frågor: Besök reserverade [instansdokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Byta ut en befintlig reserverad instans (självbetjäning)**

Du kan utbyta en reservation mot en annan reservation av samma typ. Du kan också återbetala en reservation, upp till 50 000 USD per år, om du inte längre behöver den. Funktionen för självbetjäning för byte och avbokning är inte tillgänglig för kunder med amerikanska government Enterprise Agreement. Andra abonnemangstyper för myndigheter i USA, bland annat Betala efter du-går och CSP stöds. Du måste ha ägaråtkomst i reservationsbeställningen för att kunna byta eller återbetala en befintlig reservation.

Följande steg vägleder dig om proceduren för att slutföra transaktionen

1.Logga in på din [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj de bokningar som du vill återbetala och klicka på **Exchange** 2.Välj den VM-produkt som du vill köpa och ange ett antal. Kontrollera att totalsumman för nytt köp är mer än den returnerade summan [Fastställ rätt storlek innan du köper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Granska och slutför transaktionen

**Återbetalning för en reserverad instans**

Om du vill återbetala en reservation går du till **Reservationsinformation** och klickar på **Återbetalning**

**Återbetalning klassificerad:**

**Exempel på ersättning och minimikrav för återbetalning och byte** Exempel på förhandsbokning:

- Du köper en ettårig ri för $120 den 1 januari
- Den 7 april vill du återbetala eller byta den här reservationen
- Eftersom reservationen har varit live i 97 dagar, får du (1-97/365) * $120 tillbaka. (88,1 kr). Återbetalningen är för närvarande inte återbetalningsbar
- Om du utbyter bör ditt nya köp vara större än 88,1 usd
- Återbetalningen är inte återbetalningsbar just nu

**Exempel på reservation av faktureringsplan:**

- Du köper en ettårig RI för 10 USD per månad
- Den 7 april vill du återbetala eller byta den här reservationen
- Eftersom den senaste betalningen inträffade i 7 dagar får du (1-7/31) * 100 kr tillbaka. (t.ex. 7,74 kr)
- De framtida betalningarna är 80 kr. Återbetalningen är för närvarande inte återbetalningsbar
- Återbetalningen dras av från 87,74 USD från att du har en återbetalningsgräns på 500 000 kr
- Vid utbyte ska det totala värdet av ett nytt köp vara större än 877,74 kr

**Det går inte att se fakturan för den senaste faktureringsperioden**

Några möjliga orsaker till att du inte ser en faktura:

- Du har ett månatligt kreditbelopp för prenumerationen som du inte har överskridit eller om du har en kostnadsfri utvärderingsversion. En faktura genereras endast när du är skyldig att betala pengar
- Det är mindre än 30 dagar från det att du prenumererade på Azure
- Fakturan har inte genererats än. Vänta till slutet av faktureringsperioden
- Om du inte är kontoadministratör kanske äldre fakturor inte är tillgängliga för dig

**Ladda ned fakturan från Azure Portal (.pdf)**

- Välj din prenumeration på [sidan Prenumerationer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure Portal som användare med åtkomst [till fakturor](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Välj **Fakturor**
- Klicka **på Ladda ned faktura** om du vill visa en kopia av PDF-fakturan. Om det **står Inte tillgänglig** går du till Varför visas inte en faktura för den senaste [faktureringsperioden?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Få din faktura via e-post (.pdf)**

- Välj din prenumeration på [sidan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Prenumerationer. Klicka på **Fakturor** och skicka fakturan via e-post
- Klicka **på registrera** dig och godkänn villkoren. Du måste registrera dig för varje prenumeration som du äger

Obs! Om du inte får något e-postmeddelande när du har följt anvisningarna kontrollerar du att din e-postadress är rätt i [kommunikationsinställningarna i din profil](https://account.windowsazure.com/profile)

**Ladda ned dina användningsdata från Azure Portal**

- Logga in på [Azure-kontocentret](https://account.windowsazure.com/Subscriptions) som [kontoadministratör](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Välj prenumerationen som du vill ha faktura- och användningsinformation för
- Välj **Faktureringshistorik**
- Välj **Visa aktuellt kontoutdrag** om du vill se en uppskattning av dina avgifter vid den tid då uppskattningen skapades
- Välj **Ladda ned användning** för att ladda ned dagliga användningsdata som en CSV-fil. Om du ser två versioner tillgängliga laddar du ned version 2

Andra frågor: [Besök reserverade instansdokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Rekommenderade dokument**

- [Grunderna för fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå hur rabatten för reserverade instanser tillämpas](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ladda ned eller visa din Azure-faktura och daglig användningsdata](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå hur rabatten för reserverade instanser tillämpas](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå reserverad användning av en instans för din prenumeration med betalning efter användning](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå reserverad instans-användning för företagsregistrering](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kostnader för Windows-programvara ingår inte i reserverade instanser](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverade instanser i leverantörsprogrammet för partner central molnlösning (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)