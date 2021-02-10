---
title: Distribuera AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177715"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="ca691-102">Distribuera AD FS</span><span class="sxs-lookup"><span data-stu-id="ca691-102">Deploy AD FS</span></span>

<span data-ttu-id="ca691-103">En AD FS-distribution (Active Directory Federation Services) använder den lokala infrastrukturen för att autentisera användare för Office 365-tjänster.</span><span class="sxs-lookup"><span data-stu-id="ca691-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="ca691-104">Med federerad inloggning kan du göra det möjligt för användare att logga in på Office 365-tjänster och SAAS-program (Programvara som en tjänst) som är integrerade med Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ca691-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ca691-105">Federerad inloggning autentiserar användare mot din lokala Active Directory via AD FS.</span><span class="sxs-lookup"><span data-stu-id="ca691-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="ca691-106">I företagsnätverket behöver användarna heller inte ange sina lösenord igen.</span><span class="sxs-lookup"><span data-stu-id="ca691-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="ca691-107">Distributionsrådgivaren för [AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) ger dig stegvisa instruktioner om hur du distribuerar en lokal AD FS-infrastruktur som autentiserar användare för Microsoft 365- och Office 365-tjänster.</span><span class="sxs-lookup"><span data-stu-id="ca691-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="ca691-108">Med den här guiden kan organisationen granska AD FS-komponenter och krav, skaffa och installera SSL-certifikat som behövs för distributionen och installera en proxyserver för webbprogram som krävs.</span><span class="sxs-lookup"><span data-stu-id="ca691-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
