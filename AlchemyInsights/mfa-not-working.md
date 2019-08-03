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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250183"
---
# <a name="issues-with-mfa"></a>Problem med MFA
Det finns ett par saker du kan kontrollera om användare inte kan logga in med flera faktor autentisering (MFA)

1. Den aktuella användaren blockeras i Azure Active Directory-Portal. Om så är fallet förautentiseringsförsök för den specifika användaren automatiskt nekas. [Följ stegen i den här artikeln för att häva blockeringen av dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Om avblockera användaren hjälpte eller om användaren inte är blockerad kan du försöka återställa MFA för användaren och de går igenom processen registrera igen. [Följ stegen i den här artikeln.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Om du aktiverade MFA och användarna kan inte logga in till icke-webbläsare-klienter som Outlook, Skype m.m. är kanske ADAL (Active Directory Authentication Library) inte aktiverat på O365-prenumeration. I det här fallet måste du ansluta till Exchange Online Powershell och köra denna cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*