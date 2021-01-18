---
title: Synkronisering av Domain Service
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885562"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="7924d-102">Synkronisering av Domain Service</span><span class="sxs-lookup"><span data-stu-id="7924d-102">Domain service synchronization</span></span>

<span data-ttu-id="7924d-103">Objekt och autentiseringsuppgifter i en Azure Active Directory Domain Services-hanterad domän kan antingen skapas lokalt i domänen eller synkroniseras från en Azure Active Directory-klient organisation.</span><span class="sxs-lookup"><span data-stu-id="7924d-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="7924d-104">När du först distribuerar Azure AD DS är en automatisk envägs synkronisering konfigurerad och initierad för att replikera objekten från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7924d-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="7924d-105">Den här enkelriktade synkroniseringen fortsätter att köras i bakgrunden för att hålla den Azure AD DS-hanterade domänen uppdaterad med eventuella ändringar från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7924d-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="7924d-106">Ingen synkronisering sker från Azure AD DS tillbaka till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7924d-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="7924d-107">Mer information om synkronisering av Azure Active Directory Domain Service finns i [synkronisering av Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="7924d-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
