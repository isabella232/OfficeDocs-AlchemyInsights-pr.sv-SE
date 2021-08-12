---
title: Felsöka problem med gästanvändare
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939397"
---
# <a name="troubleshoot-guest-user-issues"></a>Felsöka problem med gästanvändare

1. Anvisningar om hur du hanterar gäståtkomst till program finns i Hantera [gäståtkomst med Azure AD-åtkomstgranskningar.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Lägga till gästanvändare i katalogen i [Azure Portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)I den här snabbstarten lägger du till en ny gästanvändare i Azure AD-katalogen via Azure-portalen, skickar en inbjudan och ser hur gästanvändarens inlösningsprocess ser ut.
1. [Lägga till en gästanvändare med PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)I den här snabbstarten använder du kommandot New-AzureADMSInvitation till att lägga till en gästanvändare i Azure-klienten.
1. Mer information om hur du tilldelar användare och grupper till företagsprogram i Azure Active Directory (Azure AD), antingen från Azure-portalen eller med hjälp av PowerShell finns i Hantera användartilldelning för en [app i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B-samarbete fungerar med de flesta appar som integreras med Azure AD. I den [här artikeln](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)går vi igenom instruktioner för hur du konfigurerar några populära SaaS-appar för användning med Azure AD B2B.
1. Eftersom det är en organisation som använder B2B-samarbetsfunktioner för Azure Active Directory (Azure AD) för att bjuda in gästanvändare från partnerorganisationer till din Azure AD kan du nu ge dessa B2B-användare åtkomst till lokala appar. De här lokala apparna kan använda SAML-baserad autentisering eller integrerad Windows-autentisering (IWA) med Kerberos-begränsad delegering (KCD). Mer information finns i [Bevilja B2B-användare i Azure AD åtkomst till dina lokala program.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Lär dig hur [du beviljar lokalt hanterade partnerkonton åtkomst till molnresurser med Azure AD B2B-samarbete.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)