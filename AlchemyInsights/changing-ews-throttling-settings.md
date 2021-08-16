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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968395"
---
# <a name="changing-ews-throttling-settings"></a>Ändra inställningar för EWS-begränsning

Kör vårt automatiska test så att du kan ändra begränsningsprincipen för EWS under hela migreringen. Observera att även efter att denna har körts kommer EWS-importer fortfarande att begränsas till 150 MB per 5 minuter per postlåda; för att få högre dataflödeshastigheter för migrering bör du migrera fler användare samtidigt.

Observera att ändringar av EWS-begränsningsprincipen inte påverkar följande migreringstyper (med Microsoft-verktyg): Hybrid-, Cutover/Staged-(RPC/HTTP), IMAP, G Suite, gemensam mapp eller PST-importtjänst.