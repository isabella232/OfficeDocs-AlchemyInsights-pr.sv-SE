---
title: Konfigurera och förläng livs längd för token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917198"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="c33b1-102">Konfigurera och förläng livs längd för token</span><span class="sxs-lookup"><span data-stu-id="c33b1-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="c33b1-103">Du kan ange livs längden för en åtkomst-, SAML-eller ID-token som utfärdas av Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="c33b1-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="c33b1-104">Du kan ange livs längd för alla program i organisationen, för ett program med flera innehavare (flera organisationer) eller för ett specifikt tjänst huvud i organisationen.</span><span class="sxs-lookup"><span data-stu-id="c33b1-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="c33b1-105">Mer information finns i [konfigurations bara livs längder för token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="c33b1-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="c33b1-106">Exempel [på hur du konfigurerar livs längd för token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)finns i exempel.</span><span class="sxs-lookup"><span data-stu-id="c33b1-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="c33b1-107">Information om hur du konfigurerar livs längd och kompatibilitet för ett token i Azure Active Directory-B2C (Azure AD B2C) finns i avsnittet [Konfigurera tokens i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="c33b1-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="c33b1-108">I artikeln [Konfigurera session i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskrivs de metoder för enkel inloggning (SSO) som används i Azure AD B2C och som hjälper dig att välja den lämpligaste SSO-metoden när du konfigurerar principen.</span><span class="sxs-lookup"><span data-stu-id="c33b1-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="c33b1-109">**Hur länge tar tokens efter namn? Hur länge är de giltiga för?**</span><span class="sxs-lookup"><span data-stu-id="c33b1-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="c33b1-110">Livstiden för token är 1 timme och sessionens livstid är 24 timmar.</span><span class="sxs-lookup"><span data-stu-id="c33b1-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="c33b1-111">Det innebär att om inga förfrågningar har gjorts inom 24 timmar måste du logga in igen innan du begär en ny token.</span><span class="sxs-lookup"><span data-stu-id="c33b1-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="c33b1-112">Efter den 30 maj 2020 kan ingen ny klient organisation använda principer för konfigurerings bar token för att konfigurera sessions-och uppdateringstoken.</span><span class="sxs-lookup"><span data-stu-id="c33b1-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="c33b1-113">Utfasningen sker inom några månader efter det, vilket innebär att vi slutar att uppfylla befintliga sessioner för session och uppdatering av token.</span><span class="sxs-lookup"><span data-stu-id="c33b1-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="c33b1-114">Du kan fortfarande konfigurera livs längd för åtkomsttoken efter utfasningen.</span><span class="sxs-lookup"><span data-stu-id="c33b1-114">You can still configure access token lifetimes after the deprecation.</span></span>






