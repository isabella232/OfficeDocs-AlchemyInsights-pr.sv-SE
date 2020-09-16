---
title: Det går inte att ange eller Visa AllowSelfServicePurchase policy
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735217"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Det går inte att ange eller Visa AllowSelfServicePurchase policy

När du försöker ange eller Visa AllowSelfServicePurchase policy visas följande fel meddelande:

*HandleError: det gick inte att hämta produkt princip med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggande anslutningen avslutades: ett oväntat fel uppstod vid sändning.*

Detta kan bero på att en äldre version av Transport Layer Security (TLS). För att kunna ansluta MSCommerce-tjänsten måste du använda TLS 1,2 eller senare.  

Prova följande steg för att aktivera/ange TLS-protokollet till 1,2, verifiera och försök igen.
 1. I kommando tolken för PowerShell (PS C: \) Ange följande kommando för att ange TLS-protokollet till version 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifiera vilka TLS-protokoll som används, med följande kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Försök hämta eller uppdatera kommandona igen.

