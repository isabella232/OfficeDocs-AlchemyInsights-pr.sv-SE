---
title: Ändra inställningar för EWS-begränsning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818054"
---
# <a name="changing-ews-throttling-settings"></a>Ändra inställningar för EWS-begränsning

Kör vårt automatiska test så att du kan ändra begränsningsprincipen för EWS under hela migreringen. Observera att även efter att denna har körts kommer EWS-importer fortfarande att begränsas till 150 MB per 5 minuter per postlåda; för att få högre dataflödeshastigheter för migrering bör du migrera fler användare samtidigt.

Observera att ändringar av EWS-begränsningsprincipen inte påverkar följande migreringstyper (med Microsoft-verktyg): Hybrid-, Cutover/Staged-(RPC/HTTP), IMAP, G Suite, gemensam mapp eller PST-importtjänst.