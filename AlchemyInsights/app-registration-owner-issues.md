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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405322"
---
# <a name="app-registration-owner-issues"></a>Problem med appregistreringsägare

Här är de tillgängliga metoderna för att lägga till huvudnamn som ägare av appregistreringar:

- Använda Azure AD PowerShell-modul –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referens: [AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Använda Azure CLI - `az ad app owner add`

    Referens: [az ad-appägare](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Använda MS Graph –

    Referens: [Lägg till ägare – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Använda Azure AD-portalen – gå [till portal.azure.com](https://portal.azure.com/) > Azure Active Directory > appregistrering > Välj ditt program > ägare > Lägg till ägare

**Kan du inte visa ditt program i blad för appregistreringar trots att du är ägare till det programmet?**

Ägaren av en app är inte en administrativ roll. Om inställningen Begränsa [åtkomst till Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) är aktiverad kan bara administratören visa programmen på appregistreringsportalen. För att en ägare ska kunna visa programmen inaktiverar du den här inställningen (Ange det som NEJ) eller tilldelar administratörsrollen till ägaren för bara det specifika programmet. För detta behöver du dock en Azure AD Premium P2-licens och aktivera hantering [av privilegierad identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
