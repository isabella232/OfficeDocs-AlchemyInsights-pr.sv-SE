---
title: Autentiseringsapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405682"
---
# <a name="authentication-app"></a><span data-ttu-id="78e81-102">Autentiseringsapp</span><span class="sxs-lookup"><span data-stu-id="78e81-102">Authentication app</span></span>

<span data-ttu-id="78e81-103">Om du är global administratör kan du snabbt ta reda på vad som har hänt eller diagnostisera problem relaterade till inloggning med [inloggningsdiagnostik.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="78e81-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="78e81-104">Starta diagnostiken genom att klicka på knappen[Starta](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)diagnostik.</span><span class="sxs-lookup"><span data-stu-id="78e81-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="78e81-105">Leta reda på händelsen du vill analysera genom att ange den information du har om användaren, programmet, tiden för inloggning, begärans-ID eller korrelations-ID.</span><span class="sxs-lookup"><span data-stu-id="78e81-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="78e81-106">Granska diagnostikresultatet som visar information om vad som har hänt och vilka åtgärder du kan vidta för att göra ändringar, om några ändringar behövs.</span><span class="sxs-lookup"><span data-stu-id="78e81-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="78e81-107">**Kontrollera det scenario som är tillämpligt:**</span><span class="sxs-lookup"><span data-stu-id="78e81-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="78e81-108">Om en användare inte får ett push-meddelande i Microsoft Authenticator-appen kontrollerar du att de inte visas under MFA-blockerade användare enligt beskrivningen i Blockera och tillåta [användare.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="78e81-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="78e81-109">Om användaren inte blockeras för MFA men inte får ett push-meddelande kan de öppna appen Microsoft Authenticator, vilket hämtar väntande godkännandebegäranden.</span><span class="sxs-lookup"><span data-stu-id="78e81-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="78e81-110">Som alternativ inloggningsmetod kan användaren även klicka på Logga in på ett annat sätt och välja att använda en verifieringskod från min mobilapp.</span><span class="sxs-lookup"><span data-stu-id="78e81-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="78e81-111">Appen Microsoft Authenticator är den enda metoden för många användare.</span><span class="sxs-lookup"><span data-stu-id="78e81-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="78e81-112">[Läs mer om standardinställningar för säkerhet](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), läs Vanliga frågor och svar om [Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) för vanliga frågor och hur du löser dem.</span><span class="sxs-lookup"><span data-stu-id="78e81-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="78e81-113">**Rekommenderade videor**</span><span class="sxs-lookup"><span data-stu-id="78e81-113">**Recommended Videos**</span></span>

<span data-ttu-id="78e81-114">[Konfigurera Authenticator-appen på en ny telefon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="78e81-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
