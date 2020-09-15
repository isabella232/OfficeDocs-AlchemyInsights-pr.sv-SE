---
title: Ett av dina lokala Federations tjänst certifikat upphör att gälla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673515"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="ccef5-102">Ett av dina lokala Federations tjänst certifikat upphör att gälla</span><span class="sxs-lookup"><span data-stu-id="ccef5-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="ccef5-103">Lös problemet genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="ccef5-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="ccef5-104">Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad).</span><span class="sxs-lookup"><span data-stu-id="ccef5-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="ccef5-105">För att göra det går du till [Azure Active Directory PowerShell för Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="ccef5-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="ccef5-106">Följ anvisningarna i "Scenario 1: certifikatet för token-signerings certifikat för AD FS upphörde att gälla" i ["det uppstod ett problem vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="ccef5-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="ccef5-107">Följ anvisningarna i så här [uppdaterar eller reparerar du inställningarna för en federerad domän i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="ccef5-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="ccef5-108">Mer information om hur du förnyar Federations certifikat finns i [certifikat förnyelse för O365 och Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="ccef5-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

