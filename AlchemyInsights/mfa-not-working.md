---
title: Problem med MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810502"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="6abb5-102">Problem med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="6abb5-102">Issues with Azure MFA</span></span>
<span data-ttu-id="6abb5-103">Det finns några saker du kan kontrollera om användare inte kan logga in med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="6abb5-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="6abb5-104">Den aktuella användaren kan blockeras i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="6abb5-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="6abb5-105">Om så är fallet nekas autentiseringsförsök för den specifika användaren automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6abb5-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="6abb5-106">Följ anvisningarna i den här artikeln för att ta bort blockeringen.</span><span class="sxs-lookup"><span data-stu-id="6abb5-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="6abb5-107">Om blockeringen av användaren inte hjälpte eller om användaren inte blockeras kan du försöka återställa MFA för användaren så att han eller hon går igenom registreringsprocessen igen.</span><span class="sxs-lookup"><span data-stu-id="6abb5-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="6abb5-108">Följ anvisningarna i den här artikeln.</span><span class="sxs-lookup"><span data-stu-id="6abb5-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="6abb5-109">Om det är första gången du aktiverade MFA och användarna inte kan logga in på klienter som inte är webbläsarna, till exempel Outlook, Skype osv, kanske ADAL (Active Directory Authentication Library) inte är aktiverat i din O365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="6abb5-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="6abb5-110">I det här fallet måste du ansluta till Exchange Online Powershell och köra den här cmdleten:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="6abb5-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>