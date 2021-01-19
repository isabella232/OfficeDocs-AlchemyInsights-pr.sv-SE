---
title: Problem med att logga in på program
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901324"
---
# <a name="issues-signing-in-to-applications"></a>Problem med att logga in på program

Utför följande steg för att upptäcka orsaken till att problem som är relaterade till inloggning för användare identifieras:

1. Starta [inloggnings diagnosen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Hitta den händelse du vill analysera genom att ange informationen du har om användaren, programmet, tiden för inloggning, begärande-ID eller korrelations-ID.
3. Granska de diagnostiska resultaten som visar information om vad som hände och vilka åtgärder du kan vidta för att göra ändringar, om det behövs.

Här följer några vanliga problem som kan uppstå när du loggar in på program:

1. Du eller användaren **har slutfört en Azure AD-inloggning men ser en oväntad uppmaning** – se Artikelernas [oväntade medgivande meddelande när du loggar in på ett program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) och [oväntat fel när du godkänner ett program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Du eller en användare **har loggat in i ett program direkt, men kan inte logga in på den från en deeplink på den anpassade portalen eller åtkomst panelen**: se [Felsöka problem med att logga in i ett program från Azure AD-appar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Du eller en användare **har slutfört en Azure AD-inloggning men programmet visar ett fel meddelande och låter inte användaren slutföra inloggnings flödet**: problemet är att appen inte accepterade svaret som Azure AD gav. Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) för att felsöka.
4. Du eller en användare **kan inte logga in i ett program som inte är ett galleri som har kon figurer ATS för enkel inloggning**: Följ anvisningarna i [de här stegen](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) för att felsöka.
5. Du eller en användare **kan inte logga in på ett Azure AD Gallery-program som är konfigurerat för enkel inloggning med lösen ord**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) för att felsöka.
6. Du eller en användare **kan inte logga in i ett Microsoft-program**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) för att felsöka.
7. Du eller en användare **kan inte logga in i ett program som inte är ett galleri som har kon figurer ATS för fristående enkel inloggning**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) för att felsöka.
8. Du eller en användare **kan inte logga in på ett Azure AD Gallery-program som är konfigurerat för federerad enkel inloggning**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) för att felsöka.
9. Du eller en användare **kan inte logga in i ett anpassat program**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) för att felsöka.
10. Du eller en användare **kan inte logga in på ett lokalt program med Azure AD Application Proxy**: Följ [de här anvisningarna](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) för att felsöka.

