---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685616"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="66f90-102">Blockerar bakåtkompatibel-verifikation</span><span class="sxs-lookup"><span data-stu-id="66f90-102">Blocking legacy authentication</span></span>

<span data-ttu-id="66f90-103">Bakåtkompatibel-verifikation är en term som hänvisar till en autentiseringsbegäran som görs av:</span><span class="sxs-lookup"><span data-stu-id="66f90-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="66f90-104">Äldre Office-klienter som inte använder modern (till exempel Office 2010-klient).</span><span class="sxs-lookup"><span data-stu-id="66f90-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="66f90-105">Alla klienter som använder äldre e-postprotokoll, till exempel IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="66f90-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="66f90-106">Mer information om hur du blockerar bakåtkompatibel-inloggningsautentisering och aktiverar modern verifikation finns i [blockera bakåtkompatibel-verifikation](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="66f90-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="66f90-107">Säkerhets standarder i Azure Active Directory (Azure AD) gör det enklare att skydda din organisation.</span><span class="sxs-lookup"><span data-stu-id="66f90-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="66f90-108">Säkerhets standarder innehåller förkonfigurerade säkerhets inställningar för vanliga angrepp.</span><span class="sxs-lookup"><span data-stu-id="66f90-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="66f90-109">Mer information om säkerhets inställningar finns i [Vad är säkerhets standarder?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="66f90-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="66f90-110">**Obs!** om klient organisationen skapades på eller efter oktober 22 2019, är det möjligt att du stöter på den nya säkra standarden och redan har säkerhets standarden aktiverat i klient organisationen.</span><span class="sxs-lookup"><span data-stu-id="66f90-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="66f90-111">I en ansträngning för att skydda alla våra användare kommer säkerhets standarderna att distribueras till alla nya klient organisationer.</span><span class="sxs-lookup"><span data-stu-id="66f90-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
