---
title: Ändra inställningar för EWS-begränsning
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075915"
---
# <a name="changing-ews-throttling-settings"></a>Ändra inställningar för EWS-begränsning

Kör vårt automatiska test så att du kan ändra begränsningsprincipen för EWS under hela migreringen. Observera att även efter att denna har körts kommer EWS-importer fortfarande att begränsas till 150 MB per 5 minuter per postlåda; för att få högre dataflödeshastigheter för migrering bör du migrera fler användare samtidigt.

Observera att ändringar av EWS-begränsningsprincipen inte påverkar följande migreringstyper (med Microsoft-verktyg): Hybrid-, Cutover/Staged-(RPC/HTTP), IMAP, G Suite, gemensam mapp eller PST-importtjänst.