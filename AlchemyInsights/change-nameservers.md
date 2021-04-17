---
title: Ändra namnservrar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818630"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Uppdatera dina domännamnservrar så att de pekar på Microsoft

Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.
  
Om du vill konfigurera din domän i Microsoft 365 måste du uppdatera dina namnservrar hos registratorn. Skapa eller redigera dina namnserverposter hos din domänregistrator.
  
1. Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.
  
2. Skapa eller redigera två namnserverposterna så att de matchar följande värden:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Spara ändringar.

Du kan också hitta detaljerade instruktioner i den här artikeln: [Ändra namnservrar hos valfri domänregistrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  