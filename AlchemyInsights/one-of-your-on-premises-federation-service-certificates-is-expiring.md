---
title: En lokal Federation Service certifikat löper ut
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543727"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="24d4a-102">En lokal Federation Service certifikat löper ut</span><span class="sxs-lookup"><span data-stu-id="24d4a-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="24d4a-103">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="24d4a-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="24d4a-104">Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om den inte redan är installerat modulen).</span><span class="sxs-lookup"><span data-stu-id="24d4a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="24d4a-105">Genom att gå till [Azure Active Directory PowerShell för diagram](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="24d4a-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="24d4a-106">Följ stegen i den ”Scenario 1: AD FS-token-signering certifikatet gått ut” avsnitt av [”Det gick inte att komma åt webbplatsen” fel från AD FS när en federerad användare loggar in på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="24d4a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="24d4a-107">Följ stegen i t[hur du uppdaterar eller reparera inställningarna för en extern domän i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="24d4a-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="24d4a-108">Mer information om hur du förnyar certifikat Federation finns i [Förnya certifikat för O365 och Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="24d4a-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

