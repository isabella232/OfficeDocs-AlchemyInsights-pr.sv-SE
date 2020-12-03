---
title: Ta bort klient organisation
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564879"
---
# <a name="delete-tenant"></a>Ta bort klient organisation

Kontrol lera följande om du vill ta bort en Azure-annons:
- Du är global administratör för katalogen.
- Du är inte inloggad med ett konto som har standard katalogen, till exempel contoso.onmicrosoft.com i det signerade kontot, till exempel admin@contoso.onmicrosoft.com.
- Ta bort alla aktiva program i katalogen innan du raderas. Om du vill ta bort aktiva program navigerar du till program registreringar och tar bort befintliga program.
- Det finns inga aktiva abonnemang för alla Microsoft Online-tjänster, till exempel Microsoft Azure, Office 365 eller Azure AD Premium som är kopplade till katalogen. Överför dina abonnemang eller påskynda annulleringen av aktiva abonnemang via Azure-support och fakturering. Läs mer om hur du avbryter Office 365-och Azure-prenumerationer. Råd om att associera eller lägga till en befintlig prenumeration på en klient organisation finns i [associera eller lägga till ett Azure-abonnemang till din Azure AD-klient](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Det finns ingen aktiv licens. Om du vill ta bort licenser läser du [ta bort abonnemang för att ta bort licensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Det finns inga andra aktiva användare i katalogen förutom dig själv som global administratör när du försöker ta bort Azure AD. Ta bort alla andra aktiva användare och eventuella beroenden för ett anpassat domän namn i klient organisationen måste också tas bort, till exempel användare som skapats med admin@contoso.com.

Mer information om hur du:
- Ta bort "Azure Active Directory" eller "prenumeration", se [ta bort Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Ta bort program i katalogen finns i [ta bort program](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
