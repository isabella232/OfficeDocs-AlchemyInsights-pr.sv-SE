---
title: Fakturering för reserverad instans
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823171"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering för reserverad instans

Den reserverade instans köpet debiteras den betalnings metod som du väljer vid inköps tillfället. Abonnemangs typen måste vara ett företags avtal (erbjudande nummer: MS-AZR-0017P), betala allt eftersom (erbjudande nummer: MS-AZR-0003P), Microsoft-kundavtal eller KRYPTOGRAFIPROVIDER.

- När det gäller en företags prenumeration dras avgifterna från den monetära åtagande personens pengar och debiteras som överliggande.
- För att betala allt eftersom-abonnemang debiteras kredit kort eller faktura betalnings metod för abonnemanget.

**Avbryter reservation**

- **Själv service:** Du kan annullera eller byta ut en reserverad instans med [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj reservation och klicka på åter betalning eller utbyte. Observera att du måste ha ägar åtkomst på reservations ordern till Exchange eller åter betalning. Till gång till reservationen gör inte att du kan fortsätta med åter betalning eller utbytet. Be reservations order ägaren ge dig ägar åtkomst till reservations ordern
- **Exchange-princip:** Du kan utbyta en reservation för en annan reservation av samma typ – det finns **inga sanktioner** för reservation Exchange. Det totala åtagandet med ny reservation ska vara större än summan av den utbytta reservationens åter betalning och framtida månads betalningar (om tillämpligt)
- **Åter betalnings policy:** Summan av åter betalning och de annullerade framtida betalningarna får inte överstiga $50 000 USD i ett rullande fönster med 12 månader. Vi **debiterar för närvarande inte något straff** för åter betalningar men kan debitera det på framtida åter betalningar

**Undantag:** Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA:

- Stöd för **API/PS/CLI** är inte tillgängligt för [självbetjänings utbyte och åter betalningar för Azure-reservationer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA: Andra amerikanska abonnemangs typer, inklusive betala allt eftersom-CSP stöds

Läs mer: [hur retur-och Exchange-transaktioner behandlas](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) mer: [utbytes-och åter betalnings policy](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) andra frågor: [besök reserverade instans dokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange en befintlig reserverad instans (själv tjänst)**

Du kan utbyta en reservation för en annan reservation av samma typ. Du kan också återbetala en reservation, upp till $50 000 USD per år, om du inte längre behöver den. Själv service för Exchange och Cancel är inte tillgängligt för kunder i USA: Andra amerikanska abonnemangs typer, inklusive betala allt eftersom-CSP stöds. Du måste ha ägar åtkomst till reservations ordern för att kunna utbyta eller återbetala en befintlig reservation.

Följ stegen nedan för att slutföra transaktionen

1. Logga in på din [Azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Välj de reservationer som du vill återbetala och klicka på **Exchange** 2. Välj den VM-produkt som du vill köpa och ange en kvantitet. Se till att den nya inköps summan är större än den total summan [bestämmer rätt storlek innan du köper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. granska och Slutför transaktionen

**Åter betalning för en reserverad instans**

Om du vill återbetala en reservation går du till **reservations uppgifter** och klickar på **åter betalning**

**Pro-betygsatt åter betalning:**

**Exempel på tekniker och minsta krav för åter betalning och utbyte** Exempel på direkt reservation:

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

**Det går inte att se faktura för den senaste fakturerings perioden**

Det kan bero på att du inte ser en faktura:

- Du har ett månads belopp på ditt abonnemang, eller om du har en gratis prov period. En faktura skapas bara när du är skyldig
- Det är mindre än 30 dagar från den dag du abonnerar på Azure
- Fakturan skapas ännu inte. Vänta till slutet av fakturerings perioden
- Om du inte är konto administratör kanske inte gamla fakturor vara tillgängliga för dig

**Ladda ned din faktura från Azure Portal (. pdf)**

- Välj ditt abonnemang på sidan [prenumerationer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure Portal som [användare med åtkomst till fakturor](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Välj **fakturor**
- Klicka på **Ladda ner faktura** för att visa en kopia av din PDF-faktura. Om det **inte är tillgängligt** , se [Varför ser jag inte en faktura för den senaste fakturerings perioden?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Ta emot din faktura via e-post (. pdf)**

- Välj ditt abonnemang på sidan [prenumerationer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Klicka på **fakturor** och skicka e-post till fakturan
- Klicka på **opt in** och godkänn villkoren. Du måste välja för varje prenumeration du äger

Obs! Om du inte får ett e-postmeddelande när du har åtgärdat anvisningarna kontrollerar du att din e-postadress är korrekt i [kommunikations inställningarna för din profil](https://account.windowsazure.com/profile)

**Ladda ned användnings data från Azure-portalen**

- Logga in på [Azure-konto Center](https://account.windowsazure.com/Subscriptions) som [konto administratör](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Välj den prenumeration som du vill använda för fakturan och informationen
- Välj **fakturerings historik**
- Välj **Visa aktuell sats** för att se en uppskattning av dina avgifter vid den tidpunkt då uppskattningen genererades
- Välj **Hämta användning** för att hämta den dagliga användnings informationen som en CSV-fil. Om du ser två versioner tillgängliga kan du ladda ned version 2

Andra frågor: [besök reserverade instans dokument](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Rekommenderade dokument**

- [Grundläggande om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå hur reserverad instans rabatt används](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ladda ned eller Visa din faktura för fakturering och daglig användnings data](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå hur reserverad instans rabatt används](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå den reserverade instans användningen för ditt abonnemang på prenumerationen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Förstå reserverad instans användning för din företags registrering](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-programkostnader som inte ingår i reserverade instanser](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverade instanser i KRYPTOGRAFIPROVIDER-programmet (partner Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)