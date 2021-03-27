---
title: Logga in automatiskt till Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398747"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="041ee-102">Logga in automatiskt till Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="041ee-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="041ee-103">Microsoft Edge använder operativsystemets standardkonto för att automatiskt logga in en användare enligt hur användarens enhet har konfigurerats.</span><span class="sxs-lookup"><span data-stu-id="041ee-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="041ee-104">Scenarierna för varje typ av enhetskonfiguration och dess beroende inloggningsprocess för användare beskrivs nedan:</span><span class="sxs-lookup"><span data-stu-id="041ee-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="041ee-105">**Enheten är hybrid/AAD-J:** Det här alternativet är tillgängligt på Windows 10, i Windows på nedåtnivå och i motsvarande serverversioner.</span><span class="sxs-lookup"><span data-stu-id="041ee-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="041ee-106">Användare loggas automatiskt in med sina Azure Active Directory-konton (AD).</span><span class="sxs-lookup"><span data-stu-id="041ee-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="041ee-107">**Enheten är domän ansluten:** Det här alternativet är tillgängligt i Windows 10, Windows på nedåtnivå och motsvarande serverversioner.</span><span class="sxs-lookup"><span data-stu-id="041ee-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="041ee-108">Användare med domänkonton loggas som standard inte in automatiskt. för att aktivera automatisk inloggning för dem, använder du **policyn ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="041ee-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="041ee-109">Om du vill aktivera automatisk inloggning för användare med Azure AD-konton kan du överväga att koppla en hybrid-anslutning till deras enheter.</span><span class="sxs-lookup"><span data-stu-id="041ee-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="041ee-110">**Operativsystemets standardkonto** är ett Microsoft-konto: Det här alternativet är tillgängligt på Windows 10 RS3 (version 1709, version 10.0.16299) och senare versioner.</span><span class="sxs-lookup"><span data-stu-id="041ee-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="041ee-111">Det är osannolikt att scenariot förekommer på företagsenheter.</span><span class="sxs-lookup"><span data-stu-id="041ee-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="041ee-112">Men om standardkontot för operativsystemet är ett Microsoft-konto loggar Microsoft Edge automatiskt in användaren med Microsoft-kontot.</span><span class="sxs-lookup"><span data-stu-id="041ee-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
