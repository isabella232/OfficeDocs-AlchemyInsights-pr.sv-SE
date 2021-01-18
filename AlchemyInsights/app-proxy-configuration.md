---
title: Konfiguration av tillämpningsproxy
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885529"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="4c112-102">Konfiguration av tillämpningsproxy</span><span class="sxs-lookup"><span data-stu-id="4c112-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="4c112-103">Information om hur du konfigurerar ett programprogram i Azure AD för att visa dina lokala program i molnet finns i [Konfigurera ett program för programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="4c112-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="4c112-104">Med enkel inloggning (SSO) kan användarna få till gång till ett program utan att autentisering flera gånger.</span><span class="sxs-lookup"><span data-stu-id="4c112-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="4c112-105">Det gör det möjligt att utföra den enskilda autentiseringsprocessen i molnet, mot Azure Active Directory och låter tjänsten eller anslutningen uppträda för att användaren ska kunna slutföra eventuella ytterligare problem med autentiseringsbegäran från programmet.</span><span class="sxs-lookup"><span data-stu-id="4c112-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="4c112-106">Mer information finns i [Konfigurera enkel inloggning till ett program för programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="4c112-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="4c112-107">Använd [den här artikeln](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) för att felsöka vanliga problem med att skapa ett nytt program för programproxy.</span><span class="sxs-lookup"><span data-stu-id="4c112-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="4c112-108">Om du har problem med att konfigurera backend-identifieringen för ditt program kan du behöva [Felsöka Kerberos-begränsade Delegerings konfiguration för programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) eller följa vägledning om hur du [konfigurerar program med PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) för att lösa problemet.</span><span class="sxs-lookup"><span data-stu-id="4c112-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
