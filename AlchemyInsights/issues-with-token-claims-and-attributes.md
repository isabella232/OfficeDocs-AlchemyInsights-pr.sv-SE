---
title: Problem med Token Claims och Attribut
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036079"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="c04dc-102">Problem med Token Claims och Attribut</span><span class="sxs-lookup"><span data-stu-id="c04dc-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="c04dc-103">**Uppdatera, konfigurera eller ta bort tokenanspråk**</span><span class="sxs-lookup"><span data-stu-id="c04dc-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="c04dc-104">Med hjälp av Azure Active Directory [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) (Azure AD) kan du anpassa anspråkstypen för rollanspråk i svarstoken som du får när du har auktoriserat en app.</span><span class="sxs-lookup"><span data-stu-id="c04dc-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="c04dc-105">Programutvecklare kan använda valfria anspråk i sina Azure AD-program för att ange vilka anspråk de vill ha i token som skickas till programmet.</span><span class="sxs-lookup"><span data-stu-id="c04dc-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="c04dc-106">Mer information finns i [Ange valfria anspråk för appen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="c04dc-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="c04dc-107">[Konfigurera gruppanspråk för program med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="c04dc-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="c04dc-108">Om du använder sömlös enkel inloggning i programmet kan du se anpassa anspråk som [utfärdats i SAML-token för företagsprogram.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="c04dc-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="c04dc-109">**Attributmappning för Claims**</span><span class="sxs-lookup"><span data-stu-id="c04dc-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="c04dc-110">Information om hur du konfigurerar principen för anspråksmappning med hjälp av PowerShell finns i Anpassa anspråk i token för en viss app i [en klientorganisation (förhandsversion).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="c04dc-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="c04dc-111">Attribut för katalogschematillägg är ett sätt att lagra ytterligare data i Azure Active Directory på användarobjekt och andra katalogobjekt, till exempel grupper, information om klientorganisationen och tjänstens huvudnamn.</span><span class="sxs-lookup"><span data-stu-id="c04dc-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="c04dc-112">Endast tilläggsattribut för användarobjekt kan användas för att förge anspråk till program.</span><span class="sxs-lookup"><span data-stu-id="c04dc-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="c04dc-113">[Med attribut för katalogschematillägg i](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) anspråk beskrivs hur du använder attribut för katalogschematillägg för att skicka användardata till program i tokenanspråk.</span><span class="sxs-lookup"><span data-stu-id="c04dc-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="c04dc-114">Mer information om tokenanspråk finns i:</span><span class="sxs-lookup"><span data-stu-id="c04dc-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="c04dc-115">Anspråk i åtkomsttoken</span><span class="sxs-lookup"><span data-stu-id="c04dc-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="c04dc-116">Anspråk i en id_token</span><span class="sxs-lookup"><span data-stu-id="c04dc-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="c04dc-117">[Anspråk som](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) du kan förvänta dig i ID-tokens och åtkomsttoken som utfärdats av Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="c04dc-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="c04dc-118">Referens för SAML-token</span><span class="sxs-lookup"><span data-stu-id="c04dc-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
