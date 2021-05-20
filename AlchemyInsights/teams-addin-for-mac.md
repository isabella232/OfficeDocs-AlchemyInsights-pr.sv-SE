---
title: Teams för Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582088"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="428a4-102">Teams för Mac</span><span class="sxs-lookup"><span data-stu-id="428a4-102">Teams add-in for Mac</span></span>

<span data-ttu-id="428a4-103">Så här felsöker du Teams tillägg för Mac-operativsystemanvändare:</span><span class="sxs-lookup"><span data-stu-id="428a4-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="428a4-104">**Steg 1:** Om du har hybrid-Exchange lokalt (2016 CU3 eller senare krävs) använder du verktyget Test-HMA.ps1 för att bekräfta att modern hybridautentisering är korrekt konfigurerad.</span><span class="sxs-lookup"><span data-stu-id="428a4-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="428a4-105">Mer information finns i Validera [modern hybridautentiseringskonfiguration för Outlook för iOS och Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="428a4-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="428a4-106">**Obs!** Använd UPN-adressformatet (till exempel [username@contoso.com](mailto:username@contoso.com)), inte domän\användarnamn.</span><span class="sxs-lookup"><span data-stu-id="428a4-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="428a4-107">Gör detta även för användare Exchange Online postlådor.</span><span class="sxs-lookup"><span data-stu-id="428a4-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="428a4-108">**Steg 2:** Be användaren gå till **Verktygskonton**  >  ... i Outlook för Mac, och leta reda på och markera kontot.</span><span class="sxs-lookup"><span data-stu-id="428a4-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="428a4-109">Bekräfta att användarnamnet som visas är i UPN-format (till exempel [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="428a4-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="428a4-110">**Steg 3:** Bekräfta att användaren är en licensierad Microsoft Teams användare.</span><span class="sxs-lookup"><span data-stu-id="428a4-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="428a4-111">Användaren måste använda Office 365 Mac-prenumeration, produktversion 16.24 eller senare.</span><span class="sxs-lookup"><span data-stu-id="428a4-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>