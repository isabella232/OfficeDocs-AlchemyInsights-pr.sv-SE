---
title: Inloggnings fel för användare
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
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901252"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="1b555-102">Inloggnings fel för användare</span><span class="sxs-lookup"><span data-stu-id="1b555-102">User sign-in errors</span></span>

<span data-ttu-id="1b555-103">**Lösa problem med inloggnings diagnosen**</span><span class="sxs-lookup"><span data-stu-id="1b555-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="1b555-104">Utför följande steg för att upptäcka orsaken till att problem som är relaterade till inloggning för användare identifieras:</span><span class="sxs-lookup"><span data-stu-id="1b555-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="1b555-105">Starta [inloggnings diagnosen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="1b555-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="1b555-106">Hitta den händelse du vill analysera genom att ange informationen du har om användaren, programmet, tiden för inloggning, begärande-ID eller korrelations-ID.</span><span class="sxs-lookup"><span data-stu-id="1b555-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="1b555-107">Granska de diagnostiska resultaten som visar information om vad som hände och vilka åtgärder du kan vidta för att göra ändringar, om det behövs.</span><span class="sxs-lookup"><span data-stu-id="1b555-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="1b555-108">**Letar du efter information om AADSTS-felkoderna som returneras från Azure Active Directory (Azure AD) säkerhetstokentjänst?**</span><span class="sxs-lookup"><span data-stu-id="1b555-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="1b555-109">Läs [den här artikeln](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS fel beskrivningar, korrigeringar och vissa föreslagna lösningar</span><span class="sxs-lookup"><span data-stu-id="1b555-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>