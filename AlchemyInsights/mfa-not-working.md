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
# <a name="issues-with-azure-mfa"></a>Problem med Azure MFA
Det finns några saker du kan kontrollera om användare inte kan logga in med multifaktorautentisering (MFA)

1. Den aktuella användaren kan blockeras i Azure Active Directory-portalen. Om så är fallet nekas autentiseringsförsök för den specifika användaren automatiskt. [Följ anvisningarna i den här artikeln för att ta bort blockeringen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Om blockeringen av användaren inte hjälpte eller om användaren inte blockeras kan du försöka återställa MFA för användaren så att han eller hon går igenom registreringsprocessen igen. [Följ anvisningarna i den här artikeln.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Om det är första gången du aktiverade MFA och användarna inte kan logga in på klienter som inte är webbläsarna, till exempel Outlook, Skype osv, kanske ADAL (Active Directory Authentication Library) inte är aktiverat i din O365-prenumeration. I det här fallet måste du ansluta till Exchange Online Powershell och köra den här cmdleten:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*