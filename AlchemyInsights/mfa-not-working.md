---
title: Problem med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755149"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="e8e71-102">Problem med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="e8e71-102">Issues with Azure MFA</span></span>
<span data-ttu-id="e8e71-103">Det finns några saker du bör kontrol lera om användare inte kan logga in med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="e8e71-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e8e71-104">Den berörda användaren kan blockeras i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="e8e71-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e8e71-105">Om så är fallet kommer autentiseringsförsök för den specifika användaren att nekas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="e8e71-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e8e71-106">Följ stegen i den här artikeln för att häva blockeringen.</span><span class="sxs-lookup"><span data-stu-id="e8e71-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e8e71-107">Om det inte hjälpte att blockera användaren eller om användaren inte är blockerad kan du försöka återställa MFA för användaren och de kommer att gå igenom registrerings processen igen.</span><span class="sxs-lookup"><span data-stu-id="e8e71-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e8e71-108">Följ anvisningarna i den här artikeln.</span><span class="sxs-lookup"><span data-stu-id="e8e71-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e8e71-109">Om det är första gången du aktiverade MFA och användarna inte kan logga in på klienter som inte är webbläsare, till exempel Outlook, Skype etc, kanske ADAL (Active Directory-autentiseringspaket) inte är aktiverat på din O365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="e8e71-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e8e71-110">I det här fallet måste du ansluta till Exchange Online PowerShell och köra denna cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="e8e71-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>