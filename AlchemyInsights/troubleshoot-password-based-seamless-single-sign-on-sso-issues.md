---
title: Felsöka lösenordsbaserade problem med enkel inloggning (SSO)
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714888"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="b18d3-102">Felsöka lösenordsbaserade problem med enkel inloggning (SSO)</span><span class="sxs-lookup"><span data-stu-id="b18d3-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="b18d3-103">Mer information om grunderna i lösenordsbaserad SSO finns i [Lösenordsbaserad autentisering med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="b18d3-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="b18d3-104">**Konfigurera lösenordsbaserad SSO**</span><span class="sxs-lookup"><span data-stu-id="b18d3-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="b18d3-105">[Konfigurera lösenordsbaserad enkel inloggning – i](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) den här artikeln finns mer information om det lösenordsbaserade SSO-alternativet.</span><span class="sxs-lookup"><span data-stu-id="b18d3-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="b18d3-106">Om programmet du lägger till kräver anpassad konfiguration och du behöver använda lösenordsbaserad SSO är den här artikeln för dig.</span><span class="sxs-lookup"><span data-stu-id="b18d3-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="b18d3-107">[Konfigurera lösenordsbaserad enkel inloggning för on-prem-appar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy har stöd för flera lägen för enkel inloggning.</span><span class="sxs-lookup"><span data-stu-id="b18d3-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="b18d3-108">Lösenordsbaserad inloggning är avsedd för program som använder ett användarnamn/lösenord för autentisering.</span><span class="sxs-lookup"><span data-stu-id="b18d3-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="b18d3-109">När du konfigurerar lösenordsbaserad inloggning för programmet måste användarna logga in på det lokala programmet en gång.</span><span class="sxs-lookup"><span data-stu-id="b18d3-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="b18d3-110">Därefter lagras inloggningsinformationen i Azure Active Directory och tilldelas automatiskt till programmet när användarna öppnar det via fjärråtkomst.</span><span class="sxs-lookup"><span data-stu-id="b18d3-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="b18d3-111">Du bör redan ha publicerat och testat programmet med Programproxy.</span><span class="sxs-lookup"><span data-stu-id="b18d3-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="b18d3-112">Om inte, följer du stegen i Publicera program med Azure AD-programproxy och fortsätter sedan konfigurationen av lösenordsbaserade SSO för on-prem-appar. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)</span><span class="sxs-lookup"><span data-stu-id="b18d3-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="b18d3-113">Information om hur du felsöker lösenordsbaserad SSO finns i [Felsöka lösenordsbaserad enkel inloggning i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="b18d3-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
