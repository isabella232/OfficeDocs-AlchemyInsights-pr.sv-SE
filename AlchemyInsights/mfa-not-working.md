---
title: Problem med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545201"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="2abd0-102">Problem med MFA</span><span class="sxs-lookup"><span data-stu-id="2abd0-102">Issues with MFA</span></span>
<span data-ttu-id="2abd0-103">Det finns ett par saker att kontrollera om användare inte kan logga in med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="2abd0-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2abd0-104">Den berörda användaren kan blockeras i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="2abd0-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2abd0-105">Om så är fallet kommer autentiseringsförsök för den specifika användaren att nekas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="2abd0-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2abd0-106">Följ stegen i den här artikeln för att häva blockeringen.</span><span class="sxs-lookup"><span data-stu-id="2abd0-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2abd0-107">Om avblockera användaren inte hjälpte eller användaren inte blockeras kan du försöka återställa MFA för användaren och de kommer att gå igenom registrera processen igen.</span><span class="sxs-lookup"><span data-stu-id="2abd0-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2abd0-108">Vänligen följ stegen i den här artikeln.</span><span class="sxs-lookup"><span data-stu-id="2abd0-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2abd0-109">Om detta är första gången du aktiverat MFA och användarna inte kan logga in på icke-webbläsare klienter som Outlook, Skype, etc, kanske ADAL (Active Directory Authentication Library) inte är aktiverat på din O365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="2abd0-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2abd0-110">I det här fallet måste du ansluta till Exchange Online PowerShell och köra denna cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="2abd0-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>