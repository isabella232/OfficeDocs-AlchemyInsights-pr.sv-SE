---
title: Ta bort klient
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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993911"
---
# <a name="delete-tenant"></a>Ta bort klient

Om du vill ta bort en Azure AD ser du till att:
- Du är global administratör i katalogen.
- Du är INTE inloggad med ett konto som har standardkatalogen, till exempel contoso.onmicrosoft.com i det inloggade kontot, till exempel admin@contoso.onmicrosoft.com.
- Ta bort alla aktiva program i katalogen innan de tas bort. Om du vill ta bort aktiva program går du till Appregistreringar och tar bort befintliga program.
- Det finns inga aktiva prenumerationer på några Microsoft Online Services, till exempel Microsoft Azure, Office 365 eller Azure AD Premium är kopplade till katalogen. Överföra dina prenumerationer eller annullera aktiva prenumerationer via Azure Support och fakturering. Läs mer om hur du avbryter Office 365 och Azure-prenumerationer. Anvisningar om hur du associerar eller lägger till en befintlig prenumeration för en klientorganisation finns i Koppla eller lägga till [en Azure-prenumeration för din Azure AD-klient.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Det finns ingen aktiv licens. Information om hur du tar bort licenser [finns i Ta bort prenumeration för att ta bort licens.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Det finns inga andra aktiva användare i katalogen utöver dig själv som global administratör när du försöker ta bort Azure AD. Ta bort alla andra aktiva användare, och beroenden av ett anpassat domännamn i klientorganisationen kommer också att behöva tas bort, till exempel användare som skapats med admin@contoso.com.

Mer information om hur du gör det finns i:
- Ta bort "Azure Active Directory" eller "prenumeration", se [Ta bort Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Information om hur du tar bort program i katalogen finns i [Ta bort program.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
