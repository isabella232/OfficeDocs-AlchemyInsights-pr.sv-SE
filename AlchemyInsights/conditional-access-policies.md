---
title: Principer för villkorsstyrd åtkomst
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706075"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="16e8c-102">Principer för villkorsstyrd åtkomst</span><span class="sxs-lookup"><span data-stu-id="16e8c-102">Conditional Access policies</span></span>

<span data-ttu-id="16e8c-103">Villkorsstyrd åtkomst är en funktion i Azure AD som gör att du kan använda kontroller på åtkomsten till appar i din miljö, allt baserat på särskilda villkor och hanterat från en central plats.</span><span class="sxs-lookup"><span data-stu-id="16e8c-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="16e8c-104">Få mer information om [Villkorsstyrd åtkomst i Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="16e8c-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="16e8c-105">**Obs!** Om din klientorganisation skapades efter den 21 oktober 2019 och du oväntat blir tillfrågad om MFA, har du troligen [säkerhetsstandarder](https://aka.ms/securitydefaults) aktiverat i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="16e8c-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="16e8c-106">**Hantera säkerhetsstandarder**</span><span class="sxs-lookup"><span data-stu-id="16e8c-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="16e8c-107">Logga in på [administrationscentret](https://go.microsoft.com/fwlink/p/?linkid=834822) som global administratör.</span><span class="sxs-lookup"><span data-stu-id="16e8c-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="16e8c-108">Gå till [egenskaper för Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="16e8c-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="16e8c-109">Längst ner på sidan väljer du **Hantera säkerhetsstandarder**.</span><span class="sxs-lookup"><span data-stu-id="16e8c-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="16e8c-110">Klicka på **Ja** för att aktivera säkerhetsstandarder eller på **Nej** för att inaktivera dem.</span><span class="sxs-lookup"><span data-stu-id="16e8c-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
