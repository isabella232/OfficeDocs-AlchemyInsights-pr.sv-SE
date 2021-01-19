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
# <a name="troubleshoot-user-consent"></a>Felsöka användar medgivande

1. Du kan konfigurera hur slutanvändarna samtycker till program genom Azure Portal eller PowerShell. Se [Inställningar för användar medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) för mer information.
1. En administratör kan även använda [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) för att ge medgivande till delegerade behörigheter för en enskild användares räkning. Mer information finns i [få åtkomst för en användare](https://docs.microsoft.com/graph/auth-v2-user).
1. [Användar medgivande fel](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): i den här artikeln diskuteras fel som kan uppstå när du samtycker till ett program. Om du felsöker oväntade frågor om medgivande som inte innehåller några fel meddelanden, se [autentiseringsmetoder för Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).