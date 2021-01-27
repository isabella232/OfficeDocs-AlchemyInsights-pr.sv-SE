---
title: Villkor för villkorlig åtkomst
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015003"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="ef3b2-102">Villkor för villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="ef3b2-102">Conditional access issues</span></span>

<span data-ttu-id="ef3b2-103">**Lösa problem med inloggnings diagnosen**</span><span class="sxs-lookup"><span data-stu-id="ef3b2-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="ef3b2-104">Du kan snabbt ta reda på vad som har hänt eller diagnostisera problem med inloggning med hjälp av [inloggnings diagnosen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="ef3b2-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="ef3b2-105">Starta inloggnings diagnosen.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="ef3b2-106">Hitta den händelse du vill analysera genom att ange informationen du har om användaren, programmet, tiden för inloggning, begärande-ID eller korrelations-ID.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="ef3b2-107">Granska de diagnostiska resultaten som visar information om vad som hände och vilka åtgärder du kan vidta för att göra ändringar (om ändringar behövs).</span><span class="sxs-lookup"><span data-stu-id="ef3b2-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="ef3b2-108">**Steg för att felsöka en inloggning**</span><span class="sxs-lookup"><span data-stu-id="ef3b2-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="ef3b2-109">Gå till inloggnings sidan för Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="ef3b2-110">Filtrera inloggnings program efter användare, tidsintervall, program, status, klient program och så vidare.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="ef3b2-111">Välj en inloggnings händelse och Visa fliken villkorsstyrd åtkomst för att se vilka principer som utvärderades.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="ef3b2-112">Klicka på raden för en princip för att Visa princip detaljerna och förstå varför den tillämpas.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="ef3b2-113">**Verktyg för att felsöka en princip för villkorsstyrd åtkomst**</span><span class="sxs-lookup"><span data-stu-id="ef3b2-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="ef3b2-114">I läget endast rapport kan du utvärdera en princip utan att påverka användare.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="ef3b2-115">Vad händer om du kan simulera inloggnings händelser och se vilka principer som gäller.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="ef3b2-116">Arbets boken insikter och rapportering visar real tids påverkan för varje princip.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="ef3b2-117">**Principer för rikt linjer**</span><span class="sxs-lookup"><span data-stu-id="ef3b2-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="ef3b2-118">Principer för rikt linjer är inaktuella.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="ef3b2-119">De tillämpas inte längre och kommer snart att tas bort från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ef3b2-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="ef3b2-120">Vi rekommenderar att du aktiverar [säkerhets standarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="ef3b2-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="ef3b2-121">Mer information om villkorlig åtkomst finns i:</span><span class="sxs-lookup"><span data-stu-id="ef3b2-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="ef3b2-122">[Metod tips för villkorlig åtkomst i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Villkor i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontroller i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Platser i villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="ef3b2-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
