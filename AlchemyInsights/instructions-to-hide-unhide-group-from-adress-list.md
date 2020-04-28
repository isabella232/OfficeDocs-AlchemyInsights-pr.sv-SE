---
title: Instruktioner för att dölja/ta fram grupp från adresslistan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908362"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="86df7-102">Dölj Microsoft 365-grupp från adresslista (GAL)</span><span class="sxs-lookup"><span data-stu-id="86df7-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="86df7-103">Om du vill dölja en Microsoft 365-grupp från adresslistor (GAL) för Exchange-klienter (till exempel Outlook eller OWA) använder du följande kommando i EXO-skalet:</span><span class="sxs-lookup"><span data-stu-id="86df7-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="86df7-104">Om du vill dölja att Microsoft 365-gruppen inte är synlig för Exchange-klienter använder du följande kommando i EXO-skalet:</span><span class="sxs-lookup"><span data-stu-id="86df7-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

