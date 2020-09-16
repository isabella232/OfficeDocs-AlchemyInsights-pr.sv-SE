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
# <a name="issues-with-azure-mfa"></a>Problem med Azure MFA
Det finns några saker du bör kontrol lera om användare inte kan logga in med multifaktorautentisering (MFA)

1. Den berörda användaren kan blockeras i Azure Active Directory-portalen. Om så är fallet kommer autentiseringsförsök för den specifika användaren att nekas automatiskt. [Följ stegen i den här artikeln för att häva blockeringen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Om det inte hjälpte att blockera användaren eller om användaren inte är blockerad kan du försöka återställa MFA för användaren och de kommer att gå igenom registrerings processen igen. [Följ anvisningarna i den här artikeln.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Om det är första gången du aktiverade MFA och användarna inte kan logga in på klienter som inte är webbläsare, till exempel Outlook, Skype etc, kanske ADAL (Active Directory-autentiseringspaket) inte är aktiverat på din O365-prenumeration. I det här fallet måste du ansluta till Exchange Online PowerShell och köra denna cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*