---
title: Problem med integrering av sömlös SSO med lokala appar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868768"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="16c04-102">Problem med integrering av sömlös SSO med lokala appar</span><span class="sxs-lookup"><span data-stu-id="16c04-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="16c04-103">Så här felsöker du problem med att integrera sömlös SSO med lokala program:</span><span class="sxs-lookup"><span data-stu-id="16c04-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="16c04-104">**Rekommenderade steg**</span><span class="sxs-lookup"><span data-stu-id="16c04-104">**Recommended steps**</span></span>

1. <span data-ttu-id="16c04-105">Om du vill konfigurera ett **lokalt program** för **enkel inloggning via tillämpningsproxy** läser du [lösen ords valv för enkel inloggning med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="16c04-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="16c04-106">**Felsöka problem med programproxy**: Vi rekommenderar att du börjar med att granska fel söknings flödet, [Felsöka Application Proxy Connector-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)för att avgöra om programproxy-kopplingar är korrekt konfigurerade.</span><span class="sxs-lookup"><span data-stu-id="16c04-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="16c04-107">Om du fortfarande har problem med att ansluta till programmet följer du fel söknings stegen i [program för fel söknings program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="16c04-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="16c04-108">Du kan [identifiera CORS-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) genom att använda följande webb läsar verktyg:</span><span class="sxs-lookup"><span data-stu-id="16c04-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="16c04-109">Starta webbläsaren och gå till webb programmet.</span><span class="sxs-lookup"><span data-stu-id="16c04-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="16c04-110">Tryck på **F12** för att visa fel söknings konsolen.</span><span class="sxs-lookup"><span data-stu-id="16c04-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="16c04-111">Försök att återskapa transaktionen och granska konsol meddelandet.</span><span class="sxs-lookup"><span data-stu-id="16c04-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="16c04-112">En CORS-överträdelse skapar ett konsol fel om ursprung.</span><span class="sxs-lookup"><span data-stu-id="16c04-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="16c04-113">Vissa CORS-problem kan inte lösas, till exempel när din app dirigerar om till login.microsoftonline.com, och åtkomsttoken upphör.</span><span class="sxs-lookup"><span data-stu-id="16c04-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="16c04-114">CORS-samtalet Miss lyckas.</span><span class="sxs-lookup"><span data-stu-id="16c04-114">The CORS call then fails.</span></span> <span data-ttu-id="16c04-115">En lösning på det här scenariot är att förlänga livs längden för åtkomsttoken, för att förhindra att den upphör att gälla under en användares session.</span><span class="sxs-lookup"><span data-stu-id="16c04-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="16c04-116">Mer information om hur du gör detta finns i [konfigurations bara livs längder för token i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="16c04-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="16c04-117">**Rekommenderade dokument**</span><span class="sxs-lookup"><span data-stu-id="16c04-117">**Recommended documents**</span></span>

- [<span data-ttu-id="16c04-118">Konfigurera enkel inloggning i ett program för programproxy</span><span class="sxs-lookup"><span data-stu-id="16c04-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="16c04-119">Enkel inloggning med SAML för lokala program med programproxy</span><span class="sxs-lookup"><span data-stu-id="16c04-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="16c04-120">Förstå och lös Azure Active Directory Application Proxy CORS-frågor</span><span class="sxs-lookup"><span data-stu-id="16c04-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="16c04-121">Felsöka konfigurationer med restriktioner för delegering av Kerberos för tillämpningsproxy</span><span class="sxs-lookup"><span data-stu-id="16c04-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)