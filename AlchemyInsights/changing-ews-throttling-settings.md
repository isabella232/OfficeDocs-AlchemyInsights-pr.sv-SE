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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="a2c5f-102">Ändra inställningar för EWS-begränsning</span><span class="sxs-lookup"><span data-stu-id="a2c5f-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="a2c5f-103">Kör vårt automatiska test så att du kan ändra begränsningsprincipen för EWS under hela migreringen.</span><span class="sxs-lookup"><span data-stu-id="a2c5f-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="a2c5f-104">Observera att även efter att denna har körts kommer EWS-importer fortfarande att begränsas till 150 MB per 5 minuter per postlåda; för att få högre dataflödeshastigheter för migrering bör du migrera fler användare samtidigt.</span><span class="sxs-lookup"><span data-stu-id="a2c5f-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="a2c5f-105">Observera att ändringar av EWS-begränsningsprincipen inte påverkar följande migreringstyper (med Microsoft-verktyg): Hybrid-, Cutover/Staged-(RPC/HTTP), IMAP, G Suite, gemensam mapp eller PST-importtjänst.</span><span class="sxs-lookup"><span data-stu-id="a2c5f-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>