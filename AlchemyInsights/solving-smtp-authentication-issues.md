---
title: Aktivera SMTP-autentisering och felsökning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077669"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Aktivera SMTP-autentisering och felsökning

Om du vill aktivera SMTP-autentisering för en postlåda eller om du får felet "Klienten är inte autentiserad", "Autentiseringen lyckades inte" eller "SmtpClientAuthentication" med koden 5.7.57 eller 5.7.3 eller 5.7.139 när du försöker vidarebefordra e-post genom att autentisera en enhet eller ett program med Microsoft 365 utför du följande tre åtgärder för att lösa problemet:

1. Inaktivera [Azure-säkerhetsstandarder genom](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) att ändra **Aktivera standardinställningar för säkerhet** till **Nej.**

    a. Logga in på Azure Portal som säkerhetsadministratör, villkorlig åtkomstadministratör eller global administratör.<BR/>
    b. Bläddra till Azure Active Directory > **Egenskaper**.<BR/>
    c. Välj **Hantera säkerhetsstandarder.**<BR/>
    d. Ställ **in Aktivera säkerhetsstandarder** på **Nej.**<BR/>
    e. Välj **Spara**.

2. [Aktivera sändning av klient-SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den licensierade postlådan.

    a. I Administrationscenter för Microsoft 365 går du **till Aktiva** användare och väljer användaren.<BR/>
    b. Gå till fliken E-post och välj **Hantera e-postprogram** under **E-postprogram.**<BR/>
    d. Kontrollera att **Autentiserad SMTP är** markerat (aktiverat).<BR/>
    e. Välj **Spara ändringar**.<BR/>

3. [Inaktivera Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) för den licensierade postlådan.

    a. Gå till Administrationscenter för Microsoft 365 och välj Användare aktiva användare i den  >  **vänstra navigeringsmenyn.**<BR/>
    b. Välj **Multifaktorautentisering**.<BR/>
    c. Markera användaren och inaktivera **Multi-Factor Auth.**<BR/>
