---
title: ADFS-Federationscertifikat upphör att gälla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737207"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a3c33-102">ADFS-Federationscertifikat upphör att gälla</span><span class="sxs-lookup"><span data-stu-id="a3c33-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a3c33-103">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="a3c33-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a3c33-104">Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad).</span><span class="sxs-lookup"><span data-stu-id="a3c33-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a3c33-105">Genom att gå till [Hantera Azure AD med hjälp av Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="a3c33-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="a3c33-106">Följ stegen i "Scenario 1: AD FS-tokensignering certifikatet har upphört att gälla" avsnittet ["Det gick inte att komma åt webbplatsen" fel från AD FS när en federerad användare loggar in på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a3c33-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="a3c33-107">Följ stegen i [Uppdatera eller reparera inställningarna för en federerad domän i Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="a3c33-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="a3c33-108">Mer information om hur du förnyar Federations certifikat finns i [förnya Federations certifikat för Office 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a3c33-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
