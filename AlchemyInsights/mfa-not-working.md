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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545201"
---
# <a name="issues-with-mfa"></a>Problem med MFA
Det finns ett par saker att kontrollera om användare inte kan logga in med multifaktorautentisering (MFA)

1. Den berörda användaren kan blockeras i Azure Active Directory-portalen. Om så är fallet kommer autentiseringsförsök för den specifika användaren att nekas automatiskt. [Följ stegen i den här artikeln för att häva blockeringen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Om avblockera användaren inte hjälpte eller användaren inte blockeras kan du försöka återställa MFA för användaren och de kommer att gå igenom registrera processen igen. [Vänligen följ stegen i den här artikeln.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Om detta är första gången du aktiverat MFA och användarna inte kan logga in på icke-webbläsare klienter som Outlook, Skype, etc, kanske ADAL (Active Directory Authentication Library) inte är aktiverat på din O365-prenumeration. I det här fallet måste du ansluta till Exchange Online PowerShell och köra denna cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*