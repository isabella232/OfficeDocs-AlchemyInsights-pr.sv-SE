---
title: Ta reda på vem som har ställt in vidarebefordran för en postlåda och hur
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988251"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ta reda på vem som har ställt in vidarebefordran för en postlåda och hur

Om extern vidarebefordran har angetts för en postlåda granskas aktiviteten som en del av Set-Mailbox-cmdleten. Så här hittar du aktiviteten i granskningsloggen:

1. Gå till [säkerhets- Office 365 för & säkerhets- och efterlevnadscenter.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök i** >  **granskningsloggsökning**.
    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Kontrollera att **fältet Aktiviteter** är inställt på Visa resultat för alla **aktiviteter** (standard). Ange datumintervallet. Du behöver inte ange ett användarnamn.
1. Välj **Sök**. Aktiviteterna visas under **Resultat.**
1. Välj **Filtrera** resultat och ange sedan **Set-mailbox** i **filterfältet** Aktivitet. Då returneras alla **Aktiviteter i Set-Mailbox.**
1. Om du vill visa informationen väljer du en aktivitet och sedan **Mer information**. Under **Parametrar** ser du den e-postadress för vidarebefordran som ställts in för postlådan. UserID **representerar** den användare som konfigurerade extern vidarebefordran för postlådan.
Mer information finns i Söka [i Office 365 granskningsloggen för att felsöka vanliga scenarier](https://go.microsoft.com/fwlink/?linkid=2103944).