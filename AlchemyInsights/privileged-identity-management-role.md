---
title: Roll för privilegie rad identitet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089150"
---
# <a name="privileged-identity-managementpim-role"></a>Rollen som privilegierad identitets hantering (PIM)

**Behörigheter beviljas inte efter aktivering av en roll**

När du aktiverar en roll i Azure AD Report Management (PIM) kan aktivering inte omedelbart spridas till alla portaler som kräver den privilegierade rollen. Ibland, även om ändringen sprids kan det hända att ändringarna inte börjar gälla omedelbart.

Om aktiveringen är försenad gör du följande:

1. Logga ut från Azure-portalen och logga sedan in igen. När du aktiverar en Azure AD-roll eller en Azure-adressresurs visas stegen i din aktivering. När alla stadier är klara visas en "Logga ut"-länk. Du kan använda den här länken för att logga ut. Detta löser de flesta fall för aktiverings fördröjning.
2. I PIM kontrollerar du att du är angiven som medlem i rollen.
3. Om du aktiverar rollen som Exchange-administratör kontrollerar du att du loggar ut och loggar in igen. Om problemet kvarstår öppnar du ett support ärende och får ett problem. Om du använder rollen som Exchange-administratör för att få åtkomst till säkerhets-och efterlevnadsprinciper finns i nästa steg.
4. Om du aktiverar en roll för att få åtkomst till säkerhets-och efterföljandekrav eller om du aktiverar SharePoint-administratörskonsolen kommer det att inträffa en viss aktiverings fördröjning från några minuter upp till några timmar. Detta är ett känt problem och vi samarbetar aktivt med dessa team för att lösa problemet så snart som möjligt.

Mer information finns i:

- [Aktivera mina Azure AD-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivera mina Azure Resource-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Behörigheter tas inte bort när du har inaktiverat en roll eller om roll aktiveringen upphör**

När du inaktiverar en roll i Azure AD-privilegierad identitets hantering eller när en aktiverings period för en roll upphör kan det bero på att du har fortsatt åtkomst.

Om inaktive ringen är fördröjd gör du följande:

1. Om du inaktiverar rollen som Exchange-administratör eller om roll aktiverings perioden går ut, och du får en avsevärd fördröjning innan behörigheterna tas bort, öppnar du ett support ärende och ber din support ingenjör att hjälpa dig att arkivera en biljett med PAM-teamet i Office om det här problemet.
2. Om aktiverings perioden har gått ut men du fortfarande har webbläsarsessionen öppen stänger du webbläsaren. Du kan fortsätta att använda rollen tills du stänger den sessionen. Detta är ett känt problem och vi tittar på en möjlig åtgärd för att aktivt återkalla varje session när aktiveringen har upphört att gälla.

Om din fördröjning är annorlunda än de här två fallen måste du öppna ett support ärende.
