---
title: Privileged Identity Management roll
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973247"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)

**Behörigheter beviljas inte efter aktivering av en roll**

När du aktiverar en roll i Azure AD Privileged Identity Management (PIM) kanske inte aktiveringen direkt sprids till alla portaler som kräver den behöriga rollen. Ibland, även om ändringen sprids, kan cachelagring av webben i en portal resultera i att ändringen inte börjar gälla omedelbart.

Om aktiveringen är fördröjd följer du de här stegen:

1. Logga ut från Azure Portal och logga sedan in igen. När du aktiverar en Azure AD-roll eller en Azure-resursroll visas de olika stegen i aktiveringen. När alla steg är slutförda visas länken Logga ut. Du kan logga ut med den här länken. Det här löser de flesta fall för fördröjning vid aktivering.
2. I PIM kontrollerar du att du är medlem i rollen.
3. Om du aktiverar administratörsrollen Exchange, se till att du loggar ut och loggar in igen. Om problemet kvarstår öppnar du ett support ärende och upphöjer detta som ett problem. Om du använder rollen Exchange för att komma åt Säkerhets- och efterlevnadscenter, se nästa steg.
4. Om du aktiverar en roll för åtkomst till Säkerhets- och efterlevnadscenter, eller om du aktiverar SharePoint-administratörsrollen, kan aktiveringen fördröjas från några minuter till några timmar. Det här är ett känt problem och vi arbetar aktivt med dessa grupper för att lösa problemet så snart som möjligt.

Mer information finns i:

- [Aktivera mina Azure AD-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivera Azure-resursroller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Behörigheter tas inte bort när du inaktiverar en roll eller rollaktiveringen upphör att gälla**

När du inaktiverar en roll i Azure AD Privileged Identity Management eller när en rollaktiveringsperiod går ut kan det finnas en fördröjning där du har fortsatt åtkomst.

Om inaktiveringen är fördröjd följer du de här stegen:

1. Om du inaktiverar rollen som Exchange-administratör eller om rollaktiveringsperioden går ut och du märker en betydande fördröjning innan behörigheterna tas bort kan du öppna ett supportärende och be supportteknikern att hjälpa dig att skapa ett ärende med PAM-teamet (Privileged Access Management) i Office om problemet.
2. Stäng webbläsaren om aktiveringsperioden har gått ut, men du fortfarande har webbläsarsessionen öppen. Du kan fortsätta att använda rollen tills du stänger sessionen. Det här är ett känt problem och vi tittar på en möjlig korrigering för att aktivt återkalla varje session när aktiveringen har upphört.

Om din fördröjning inte är samma som de här två scenarierna kan du öppna ett support ärende.
