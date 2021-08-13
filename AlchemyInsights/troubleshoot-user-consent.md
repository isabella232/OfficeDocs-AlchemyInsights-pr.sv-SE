---
title: Felsöka användarens medgivande
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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007916"
---
# <a name="troubleshoot-user-consent"></a>Felsöka användarens medgivande

1. Du kan konfigurera hur slutanvändarna samtycker till program via Azure Portal eller PowerShell. Mer information [finns i Inställningar](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) för användarmedgivande.
1. En administratör kan också använda [Microsofts Graph API för](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) att bevilja medgivande till delegerade behörigheter för en enskild användares räkning. Mer information finns i [Få åtkomst för en användare.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Fel i användarens medgivande:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)I den här artikeln beskrivs fel som kan uppstå under medgivandeprocessen för ett program. Om du felsöker uppmaningar om oväntade medgivanden som inte innehåller några felmeddelanden kan du gå till [Autentiseringsscenarier för Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)