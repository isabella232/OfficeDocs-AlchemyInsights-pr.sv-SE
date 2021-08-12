---
title: Problem med appregistreringsägare
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951151"
---
# <a name="app-registration-owner-issues"></a>Problem med appregistreringsägare

Här är de tillgängliga metoderna för att lägga till huvudnamn som ägare av appregistreringar:

- Använda Azure AD PowerShell-modul –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referens: [AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Använda Azure CLI - `az ad app owner add`

    Referens: [az ad-appägare](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Använda MS Graph -

    Referens: [Lägg till ägare – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Använda Azure AD-portalen – gå [till portal.azure.com](https://portal.azure.com/) > Azure Active Directory > appregistrering > Välj ditt program > ägare > Lägg till ägare

**Kan du inte visa ditt program i blad för appregistreringar trots att du är ägare till det programmet?**

Ägaren av en app är inte en administrativ roll. Om inställningen Begränsa [åtkomst till Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) är aktiverad kan bara administratören visa programmen på appregistreringsportalen. För att en ägare ska kunna visa programmen inaktiverar du den här inställningen (Ange det som NEJ) eller tilldelar administratörsrollen till ägaren för bara det specifika programmet. För detta krävs dock en licens för Azure AD Premium P2 och aktivera [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
