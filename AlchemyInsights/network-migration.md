---
title: Nätverkskommunikation
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799582"
---
# <a name="network-migration"></a>Nätverkskommunikation

Din O365-klient organisation är eventuellt kopplad till flera Yammer-nätverk i en 1 klient organisation: många nätverks konfiguration. Från och med den 16 oktober 2018 stöder Yammer inte längre flera Yammer-nätverk som är associerade med en klient organisation. Du kan göra en nätverks migrering för att komma till en Preferred 1:1-konfiguration.
  
- Om du vill visa en lista över de nätverk som är kopplade till din klient organisation, loggar du in på Yammer som global administratör och bläddrar till **nätverks administratör**och sedan på **nätverkskommunikation**. Välj **Nästa**.

- Om flera nätverk visas i steg 2 av 3 har du flera Yammer-nätverk kopplade till din O365-klient organisation.

- Om du vill korrigera konfigurationen för en 1:1-konfiguration fortsätter du med verktyget för nätverksdiagnostik.

- Mer information om nätverksautentisering finns i [nätverks migrering: konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).

Observera:
  
- **En nätverks migrering migrerar bara aktiva och väntande användare.** Tillsammans med aktiva användare migreras användarnas information, till exempel namn och profil bild. Allt nätverks innehåll, inklusive grupper, migreras inte.

- **Det går inte att byta nätverks överföring.** Du kommer inte att kunna komma åt ditt dotter bolag och dess innehåll efter migreringen. Så innan du funderar på att migrera kan du planera omsorgsfullt.
