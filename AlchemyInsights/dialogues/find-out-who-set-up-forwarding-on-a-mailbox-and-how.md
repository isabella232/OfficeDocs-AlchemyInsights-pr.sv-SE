---
title: Ta reda på vem som konfigurerade vidarebefordran för en postlåda och hur
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429996"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ta reda på vem som konfigurerade vidarebefordran för en postlåda och hur

Om extern vidarebefordran har angetts för en postlåda granskas aktiviteten som en del av Set-Mailbox-cmdleten. Så här hittar du aktiviteten i granskningsloggen:

1. Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Välj **Sök** >  **granskningsloggsökning.**
    > [!NOTE]
    > Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu. Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.
1. Kontrollera att fältet **Aktiviteter** är inställt på **Visa resultat för alla aktiviteter** (standard). Ange datumintervallet. Du behöver inte ange ett användarnamn.
1. Välj **Sök.** Aktiviteterna visas under **Resultat.**
1. Välj **Filtrera resultat** och ange sedan Ange postlåda **i** fältet **Aktivitetsfilter.** Då returneras **alla Aktiviteter för Uppsättningspostlåda.**
1. Om du vill visa informationen väljer du en aktivitet och sedan **Mer information.** Under **Parametrar** kan du se vidarebefordran av e-postadressen som ställts in för postlådan. **Användar-ID** representerar den användare som konfigurerade extern vidarebefordran för postlådan.
Mer information finns i Söka [i Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)