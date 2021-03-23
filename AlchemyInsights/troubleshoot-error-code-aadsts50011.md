---
title: Felsöka felkod AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038060"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="ad812-102">Felsöka felkod AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="ad812-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="ad812-103">Lös AADSTS50011-felet genom att utföra det rekommenderade steget som beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="ad812-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="ad812-104">**AADSTS50011**: InvalidReplyTo – Svarsadressen saknas, är felaktigt konfigurerad eller matchar inte svarsadresser som konfigurerats för appen.</span><span class="sxs-lookup"><span data-stu-id="ad812-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="ad812-105">Som en lösning ser du till att lägga till den här svarsadressen som saknas i Azure Active Directory-appen (AD) eller har någon som har behörighet att hantera programmet i AD gör detta åt dig.</span><span class="sxs-lookup"><span data-stu-id="ad812-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="ad812-106">Mer information finns i felsökningsartikeln för felet [AADSTS50011.](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch)</span><span class="sxs-lookup"><span data-stu-id="ad812-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>