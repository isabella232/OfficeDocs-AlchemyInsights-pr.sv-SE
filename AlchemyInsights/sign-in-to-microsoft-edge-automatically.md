---
title: Logga in i Microsoft Edge automatiskt
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678817"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="7a69c-102">Logga in i Microsoft Edge automatiskt</span><span class="sxs-lookup"><span data-stu-id="7a69c-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="7a69c-103">Microsoft Edge använder operativ systemets standard konto för att automatiskt logga in en användare baserat på hur användarens enhet är konfigurerad.</span><span class="sxs-lookup"><span data-stu-id="7a69c-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="7a69c-104">Scenarierna för varje typ av enhets konfiguration och inloggnings process som tillhör ande användare beskrivs nedan:</span><span class="sxs-lookup"><span data-stu-id="7a69c-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="7a69c-105">**Enheten är hybrid/AAD-J**: det här alternativet är tillgängligt i Windows 10, Windows och motsvarande Server versioner.</span><span class="sxs-lookup"><span data-stu-id="7a69c-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="7a69c-106">Användarna loggas automatiskt in med sina Azure Active Directory (AD)-konton.</span><span class="sxs-lookup"><span data-stu-id="7a69c-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="7a69c-107">**Enheten är** domänansluten: det här alternativet är tillgängligt i Windows 10, i Windows och motsvarande Server versioner.</span><span class="sxs-lookup"><span data-stu-id="7a69c-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="7a69c-108">Som standard är användare med domän konton inte inloggade automatiskt; Använd **ConfigureOnPremisesAccountAutoSignIn** policy för att aktivera automatisk inloggning för dem.</span><span class="sxs-lookup"><span data-stu-id="7a69c-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="7a69c-109">För att aktivera automatisk inloggning för användare med Azure AD-konton kan du välja att hybrid-ansluter till sina enheter.</span><span class="sxs-lookup"><span data-stu-id="7a69c-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="7a69c-110">**Operativ systemets standard konto är ett Microsoft-konto**: det här alternativet är tillgängligt på Windows 10 RS3 (version 1709, build 10.0.16299) och senare versioner.</span><span class="sxs-lookup"><span data-stu-id="7a69c-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="7a69c-111">Det är osannolikt att scenariot inträffar på företags enheter.</span><span class="sxs-lookup"><span data-stu-id="7a69c-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="7a69c-112">Om operativ systemets standard konto är ett Microsoft-konto loggar Microsoft Edge automatiskt in användaren med Microsoft-kontot.</span><span class="sxs-lookup"><span data-stu-id="7a69c-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
