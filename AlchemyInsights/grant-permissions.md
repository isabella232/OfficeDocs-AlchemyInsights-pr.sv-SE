---
title: Bevilja behörigheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901617"
---
# <a name="grant-permissions"></a><span data-ttu-id="e63d9-102">Bevilja behörigheter</span><span class="sxs-lookup"><span data-stu-id="e63d9-102">Grant permissions</span></span>

1. <span data-ttu-id="e63d9-103">**Bevilja klient organisations medgivande**: se [bevilja klient organisations medgivande för ett program för att](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) få stegvisa instruktioner för beviljande av klient organisationens administratörs medgivande från Azure-portalen med Azure AD PowerShell eller från meddelandet.</span><span class="sxs-lookup"><span data-stu-id="e63d9-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="e63d9-104">**Ge tillstånd för en viss användare** i stället för att bevilja godkännande för hela organisationen kan en administratör också använda [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) för att ge medgivande till delegerade behörigheter för en enskild användares räkning.</span><span class="sxs-lookup"><span data-stu-id="e63d9-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="e63d9-105">Mer information finns i [få åtkomst för en användare](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="e63d9-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>