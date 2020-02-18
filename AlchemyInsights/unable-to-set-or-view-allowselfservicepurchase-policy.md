---
title: Det går inte att ange eller visa policyn AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091774"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Det går inte att ange eller visa policyn AllowSelfServicePurchase

När du försöker ange eller visa allowSelfServicePurchase-principen visas följande felmeddelande:

*HandleError : Det gick inte att hämta produktprincipen med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggande anslutningen stängdes: Ett oväntat fel uppstod på ett skicka.*

Detta kan bero på en äldre version av Transport Layer Security (TLS). Om du vill ansluta MSCommerce-tjänsten måste du använda TLS 1.2 eller större.  

Prova följande steg för att aktivera/ange TLS-protokollet till 1.2, verifiera och försök igen.
 1. Vid kommandotolken för PowerShell\) (PS C: ange följande kommando för att ställa in TLS-protokollet till version 1.2:

    \[Net.ServicePointManager]:SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Kontrollera att TLS-protokollen används, med följande kommando:

    \[Net.ServicePointManager]:SecurityProtocol 

3. Försök igen kommandonhämta eller uppdatera efter behov.

