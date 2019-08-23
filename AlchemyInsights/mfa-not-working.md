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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545201"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="3fcc6-102">Problem med MFA</span><span class="sxs-lookup"><span data-stu-id="3fcc6-102">Issues with MFA</span></span>
<span data-ttu-id="3fcc6-103">Det finns ett par saker du kan kontrollera om användare inte kan logga in med flera faktor autentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="3fcc6-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3fcc6-104">Den aktuella användaren blockeras i Azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3fcc6-105">Om så är fallet förautentiseringsförsök för den specifika användaren automatiskt nekas.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3fcc6-106">Följ stegen i den här artikeln för att häva blockeringen av dem.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3fcc6-107">Om avblockera användaren hjälpte eller om användaren inte är blockerad kan du försöka återställa MFA för användaren och de går igenom processen registrera igen.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3fcc6-108">Följ stegen i den här artikeln.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3fcc6-109">Om du aktiverade MFA och användarna kan inte logga in till icke-webbläsare-klienter som Outlook, Skype m.m. är kanske ADAL (Active Directory Authentication Library) inte aktiverat på O365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="3fcc6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3fcc6-110">I det här fallet måste du ansluta till Exchange Online Powershell och köra denna cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="3fcc6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>