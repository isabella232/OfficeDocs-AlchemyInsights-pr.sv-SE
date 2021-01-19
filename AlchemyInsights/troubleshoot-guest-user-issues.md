---
title: Felsöka problem med gäst användare
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
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901591"
---
# <a name="troubleshoot-guest-user-issues"></a>Felsöka problem med gäst användare

1. Information om hur du hanterar gäst åtkomst till program finns i [Hantera gäst åtkomst med Azure AD Access-granskningar](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Lägga till gäst användare i din katalog i Azure-portalen](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): i det här snabb starts fönstret lägger du till en ny gäst användare i din Azure AD-katalog via Azure-portalen, skickar en inbjudan och ser vad gäst användarens inbjudan att lösa in ser ut.
1. [Lägga till en gäst användare med PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): i det här snabb starts fönstret använder du kommandot New-AzureADMSInvitation för att lägga till en gäst användare i din Azure-klient.
1. Information om hur du tilldelar användare och grupper till företags program i Azure Active Directory (Azure AD), antingen från Azure-portalen eller med PowerShell, finns i [hantera användar tilldelning för ett program i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-samarbete fungerar med de flesta appar som är integrerade med Azure AD. I den här [artikeln](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)går vi igenom anvisningar för hur du konfigurerar några populära SaaS-appar som kan användas med Azure AD B2B.
1. Som en organisation som använder Azure Active Directory (Azure AD) B2B-samarbets funktioner för att bjuda in gäst användare från partner organisationer till din Azure AD kan du nu ge dessa B2B-användare åtkomst till lokala appar. Dessa lokala appar kan använda SAML-baserad autentisering eller integrerad Windows-autentisering (IWA) med Kerberos begränsning delegering (KCD). Mer information finns i [tilldela B2B-användare i Azure AD till gång till dina lokala program](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Lär dig hur du [tilldelar lokalt hanterade partner konton åtkomst till moln resurser med Azure AD B2B-samarbete](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).