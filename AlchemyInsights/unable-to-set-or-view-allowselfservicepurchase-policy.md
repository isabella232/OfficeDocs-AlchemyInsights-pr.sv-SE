---
title: Det går inte att ange eller visa principen AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826109"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Det går inte att ange eller visa principen AllowSelfServicePurchase

När du försöker ange eller visa principen AllowSelfServicePurchase får du följande felmeddelande:

*HandleError: Det gick inte att hämta produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggande anslutningen stängdes: Ett oväntat fel uppstod vid ett skicka-meddelande.*

Det här kan bero på en äldre version av TLS (Transport Layer Security). Du måste använda TLS 1.2 eller större för att ansluta tjänsten MSCommerce.  

Prova följande steg för att aktivera/ange TLS-protokollet till 1.2, verifiera och försök igen.
 1. I PowerShell-kommandotolken (PS C: ange följande kommando för att ange \) TLS-protokollet till version 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kontrollera det eller de TLS-protokoll som används, med följande kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Försök igen med kommandona Hämta och Uppdatera efter behov.

