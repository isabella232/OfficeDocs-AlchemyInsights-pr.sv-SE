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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="34112-102">Ändra inställningar för EWS-begränsning</span><span class="sxs-lookup"><span data-stu-id="34112-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="34112-103">Kör vårt automatiska test så att du kan ändra begränsningsprincipen för EWS under hela migreringen.</span><span class="sxs-lookup"><span data-stu-id="34112-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="34112-104">Observera att även efter att denna har körts kommer EWS-importer fortfarande att begränsas till 150 MB per 5 minuter per postlåda; för att få högre dataflödeshastigheter för migrering bör du migrera fler användare samtidigt.</span><span class="sxs-lookup"><span data-stu-id="34112-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="34112-105">Observera att ändringar av EWS-begränsningsprincipen inte påverkar följande migreringstyper (med Microsoft-verktyg): Hybrid-, Cutover/Staged-(RPC/HTTP), IMAP, G Suite, gemensam mapp eller PST-importtjänst.</span><span class="sxs-lookup"><span data-stu-id="34112-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>