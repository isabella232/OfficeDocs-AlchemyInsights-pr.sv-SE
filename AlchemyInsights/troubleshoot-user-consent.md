---
title: Felsöka användar medgivande
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901628"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="4077b-102">Felsöka användar medgivande</span><span class="sxs-lookup"><span data-stu-id="4077b-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="4077b-103">Du kan konfigurera hur slutanvändarna samtycker till program genom Azure Portal eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4077b-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="4077b-104">Se [Inställningar för användar medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) för mer information.</span><span class="sxs-lookup"><span data-stu-id="4077b-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="4077b-105">En administratör kan även använda [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) för att ge medgivande till delegerade behörigheter för en enskild användares räkning.</span><span class="sxs-lookup"><span data-stu-id="4077b-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="4077b-106">Mer information finns i [få åtkomst för en användare](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="4077b-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="4077b-107">[Användar medgivande fel](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): i den här artikeln diskuteras fel som kan uppstå när du samtycker till ett program.</span><span class="sxs-lookup"><span data-stu-id="4077b-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="4077b-108">Om du felsöker oväntade frågor om medgivande som inte innehåller några fel meddelanden, se [autentiseringsmetoder för Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="4077b-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>