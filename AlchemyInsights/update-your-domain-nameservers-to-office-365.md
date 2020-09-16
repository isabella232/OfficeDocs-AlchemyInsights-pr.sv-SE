---
title: Uppdatera dina domännamnservrar så att de pekar på Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734929"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Uppdatera dina domännamnservrar så att de pekar på Microsoft

Obs! Ändringar av namnservern kan ibland ta upp till 48 timmar att distribuera.
  
För att konfigurera din domän hos Microsoft måste namnservrar hos din registrator uppdateras. Skapa eller redigera dina namnserverposter hos din domänregistrator.
  
1. Gå till din domänregistrators webbplats och leta reda på var du kan redigera namnservrarna.

2. Skapa eller redigera två namnserverposterna så att de matchar följande värden:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Spara ändringar.

Detaljerade anvisningar finns i den här artikeln: [ändra namnservrar för att konfigurera Microsoft 365 med valfri domän registrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  