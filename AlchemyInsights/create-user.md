---
title: Skapa användare
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896733"
---
# <a name="create-user"></a>Skapa användare

**MEDDELANDE:**

- [Utfasning av WebView-inloggningssupport från Google från och med den 4 januari 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testa om dina appar kan påverkas av att [följa Googles anvisningar](https://go.microsoft.com/fwlink/?linkid=2157323) om kompatibilitetstestning.
- Kontrollera att du använder systemets webbvy eller systemwebbläsare när du loggar in dina användare med Google-konsumentkonton. Mer information finns i [Problem med att logga in på program med bara Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Jag kan inte skapa en ny användare i min Azure AD-katalog**

1. Se till att du har behörighet att skapa en ny standardanvändare. Endast rollen global administratör eller användaradministratör i Azure Active Directory (AD) kan skapa en ny standardanvändare. Om du inte har någon av dessa roller kan du be en administratör att lägga till dig i en av rollerna eller att skapa det nya användarkontot åt dig.
1. Kontrollera att användarnamnet finns i en domän som har verifierats i Azure AD. Om du inte har några verifierade anpassade domännamn i azure AD kan du använda din initiala Azure AD-domän, som slutar med *.onmicrosoft.com.
1. Kontrollera att användarnamnet finns i en domän som inte är federerad till Azure AD från din lokala AD. Användare kan inte läggas till i molnet med domännamn som är externa från lokalt.
1. Kontrollera att ingen annan användare eller kontakt redan har det användarnamn som du vill tilldela den nya användaren. Användarnamn måste vara unika för alla Azure AD.
1. Se [Azure AD-roller och -administratörer](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) för Azure AD.
1. Se [domännamnen för](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. Granska [granskningsloggar](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) om du vill se mer detaljerad information om en nyligen skapad eller borttagna användare, till exempel vem som utförde åtgärden och när.
1. Mer information om hur du lägger till nya användare finns [i Använda Azure Portal för att skapa en ny användare i azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD-administratörsroller:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Administratörsrollbehörigheter i Azure Active Directory
1. Du kan också [använda Azure AD PowerShell för att skapa en ny användare.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
