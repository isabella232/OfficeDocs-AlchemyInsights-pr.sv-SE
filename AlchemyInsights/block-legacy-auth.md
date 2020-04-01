---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079278"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="b421a-102">Blockera äldre autentisering</span><span class="sxs-lookup"><span data-stu-id="b421a-102">Blocking legacy authentication</span></span>

<span data-ttu-id="b421a-103">Äldre autentisering är en term som refererar till en autentiseringsbegäran som gjorts av:</span><span class="sxs-lookup"><span data-stu-id="b421a-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="b421a-104">Äldre Office-klienter som inte använder modern autentisering (till exempel Office 2010-klient).</span><span class="sxs-lookup"><span data-stu-id="b421a-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="b421a-105">Alla klienter som använder äldre e-postprotokoll som IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="b421a-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="b421a-106">Mer information om hur du blockerar äldre autentisering och aktiverar modern autentisering finns i [Blockera äldre autentisering](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="b421a-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="b421a-107">Standardvärden för säkerhet i Azure Active Directory (Azure AD) gör det enklare att vara säker och skydda din organisation.</span><span class="sxs-lookup"><span data-stu-id="b421a-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="b421a-108">Standardinställningar för säkerhet innehåller förkonfigurerade säkerhetsinställningar för vanliga attacker.</span><span class="sxs-lookup"><span data-stu-id="b421a-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="b421a-109">Mer information om standardvärden för säkerhet finns i [Vad är standardvärden för säkerhet?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="b421a-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="b421a-110">**Om**din klient skapades den 22 oktober 2019 eller senare är det möjligt att du upplever det nya beteendet för säker som standard och redan har aktiverat säkerhetsstandardinställningar i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="b421a-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="b421a-111">I ett försök att skydda alla våra användare distribueras säkerhetsinställningar till alla nya klienter som skapas.</span><span class="sxs-lookup"><span data-stu-id="b421a-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
