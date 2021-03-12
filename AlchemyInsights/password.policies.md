---
title: Lösenordsprinciper
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747054"
---
# <a name="password-policies"></a><span data-ttu-id="7bafa-102">Lösenordsprinciper</span><span class="sxs-lookup"><span data-stu-id="7bafa-102">Password policies</span></span>

<span data-ttu-id="7bafa-103">**Jag har problem med lösenordsprincipen för en användare**</span><span class="sxs-lookup"><span data-stu-id="7bafa-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="7bafa-104">Lösenordsprincipen för en användare beror på om användaren endast är molnbaserad eller lokal.</span><span class="sxs-lookup"><span data-stu-id="7bafa-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="7bafa-105">Endast användare i molnet måste välja ett lösenord som uppfyller kraven i den här artikeln: [Lösenordsprinciper som endast gäller för molnanvändarkonton](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="7bafa-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="7bafa-106">Lokala användare måste välja ett lösenord som uppfyller de lokala kraven.</span><span class="sxs-lookup"><span data-stu-id="7bafa-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="7bafa-107">Om en lokal användare inte kan ange sitt lösenord ska du kontrollera dina lokala krav.</span><span class="sxs-lookup"><span data-stu-id="7bafa-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="7bafa-108">**Jag vet inte hur jag anger eller kontrollerar förfalloprinciper för lösenord**</span><span class="sxs-lookup"><span data-stu-id="7bafa-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="7bafa-109">Du kan ange och kontrollera förfalloprincipen för molnanvändare i klientorganisationen med hjälp av PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7bafa-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="7bafa-110">Följ anvisningarna i den här artikeln: [Ange eller kontrollera lösenordsprinciper med hjälp av PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="7bafa-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="7bafa-111">Förfalloprincipen för lösenord för lokala användare anges i din lokala AD.</span><span class="sxs-lookup"><span data-stu-id="7bafa-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="7bafa-112">**Andra användbara länkar:**</span><span class="sxs-lookup"><span data-stu-id="7bafa-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="7bafa-113">Komma igång med återställning av lösenord</span><span class="sxs-lookup"><span data-stu-id="7bafa-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="7bafa-114">Felsöka administratörsinitierad lösenordsåterställning</span><span class="sxs-lookup"><span data-stu-id="7bafa-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
