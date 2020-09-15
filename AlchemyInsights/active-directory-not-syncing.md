---
title: Active Directory synkroniserar inte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697647"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="6bc3b-102">Active Directory synkroniserar inte</span><span class="sxs-lookup"><span data-stu-id="6bc3b-102">Active Directory not syncing</span></span>

<span data-ttu-id="6bc3b-103">Om du får synkroniseringsfel, till exempel "ingen senaste synkronisering" eller Observera att status för katalog synkroniseringen i administrations portalen för Office visar "senast synkroniserat för mer än 3 dagar sedan", kan det bero på att AADConnect har felaktiga inställningar eller otillräcklig behörighet att utföra en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="6bc3b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="6bc3b-104">Det kan lösa problemet snabbt genom att installera om AADConnect med hjälp av snabb inställningar:</span><span class="sxs-lookup"><span data-stu-id="6bc3b-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="6bc3b-105">[Ladda ner den senaste versionen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="6bc3b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="6bc3b-106">[Följ anvisningarna för snabb installationen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="6bc3b-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="6bc3b-107">Mer information om AADConnect-tjänst konton finns i [Azure AD Connect: accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="6bc3b-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
