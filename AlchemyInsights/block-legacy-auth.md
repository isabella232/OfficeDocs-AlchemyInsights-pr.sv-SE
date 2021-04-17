---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820196"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="d4fec-102">Blockera äldre autentisering</span><span class="sxs-lookup"><span data-stu-id="d4fec-102">Blocking legacy authentication</span></span>

<span data-ttu-id="d4fec-103">Äldre autentisering är en term som refererar till en autentiseringsbegäran som görs av:</span><span class="sxs-lookup"><span data-stu-id="d4fec-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="d4fec-104">Äldre Office-klienter som inte använder modern autentisering (till exempel Office 2010-klient).</span><span class="sxs-lookup"><span data-stu-id="d4fec-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="d4fec-105">Alla klienter som använder äldre e-postprotokoll, till exempel IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="d4fec-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="d4fec-106">Mer information om hur du blockerar äldre autentisering och aktiverar modern autentisering finns i [Blockera äldre autentisering.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="d4fec-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="d4fec-107">Standardvärden för säkerhet i Azure Active Directory (Azure AD) gör det enklare att vara säker och skydda organisationen.</span><span class="sxs-lookup"><span data-stu-id="d4fec-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="d4fec-108">Säkerhetsstandarder innehåller förkonfigurerade säkerhetsinställningar för vanliga attacker.</span><span class="sxs-lookup"><span data-stu-id="d4fec-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="d4fec-109">Mer information om säkerhetsstandarder finns i Vad [är standardinställningar](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)för säkerhet? .</span><span class="sxs-lookup"><span data-stu-id="d4fec-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="d4fec-110">**Obs!** Om klientorganisationen skapades den 22 oktober 2019 eller efter den 22 oktober 2019 är det möjligt att du upplever det nya säkerhetsbeteendet som standard och redan har aktiverat säkerhetsstandarder i klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="d4fec-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="d4fec-111">I syfte att skydda alla våra användare distribueras säkerhetsstandarder till alla nya klientorganisationar som skapas.</span><span class="sxs-lookup"><span data-stu-id="d4fec-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
