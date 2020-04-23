---
title: Ett av dina lokala federationsservicecertifikat löper ut
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785321"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="b9b4d-102">Ett av dina lokala federationsservicecertifikat löper ut</span><span class="sxs-lookup"><span data-stu-id="b9b4d-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="b9b4d-103">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="b9b4d-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="b9b4d-104">Installera Microsoft Azure Active Directory Module för Windows PowerShell på datorn (om modulen inte redan är installerad).</span><span class="sxs-lookup"><span data-stu-id="b9b4d-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="b9b4d-105">Det gör du genom att gå till [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="b9b4d-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="b9b4d-106">Följ stegen i avsnittet "Scenario 1: AD FS-tokensigneringscertifikatet har upphört att gälla" i [felet "Det uppstod ett problem med att komma åt webbplatsen" från AD FS när en federerad användare loggar in på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="b9b4d-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="b9b4d-107">Följ stegen i [Så här uppdaterar eller reparerar du inställningarna för en federerad domän i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="b9b4d-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="b9b4d-108">Mer information om hur du förnyar federationscertifikat finns i [Förnyelse av certifikat för O365 och Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="b9b4d-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

