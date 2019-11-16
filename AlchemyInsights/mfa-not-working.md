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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768855"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="e5452-102">Problem med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="e5452-102">Issues with Azure MFA</span></span>
<span data-ttu-id="e5452-103">Det finns ett par saker att kontrollera om användare inte kan logga in med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="e5452-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e5452-104">Den berörda användaren kan blockeras i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="e5452-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e5452-105">Om så är fallet kommer autentiseringsförsök för den specifika användaren att nekas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="e5452-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e5452-106">Följ stegen i den här artikeln för att häva blockeringen.</span><span class="sxs-lookup"><span data-stu-id="e5452-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e5452-107">Om avblockera användaren inte hjälpte eller användaren inte blockeras kan du försöka återställa MFA för användaren och de kommer att gå igenom registrera processen igen.</span><span class="sxs-lookup"><span data-stu-id="e5452-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e5452-108">Vänligen följ stegen i den här artikeln.</span><span class="sxs-lookup"><span data-stu-id="e5452-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e5452-109">Om detta är första gången du aktiverat MFA och användarna inte kan logga in på icke-webbläsare klienter som Outlook, Skype, etc, kanske ADAL (Active Directory Authentication Library) inte är aktiverat på din O365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="e5452-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e5452-110">I det här fallet måste du ansluta till Exchange Online PowerShell och köra denna cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="e5452-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>