---
title: ADFS Federation Certificate Expiring
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821969"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="5c6fa-102">ADFS Federation Certificate Expiring</span><span class="sxs-lookup"><span data-stu-id="5c6fa-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="5c6fa-103">Lös problemet genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="5c6fa-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="5c6fa-104">Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad).</span><span class="sxs-lookup"><span data-stu-id="5c6fa-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="5c6fa-105">Det gör du genom att gå [till Hantera Azure AD med Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="5c6fa-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="5c6fa-106">Följ anvisningarna i avsnittet "Scenario 1: AD FS-token-signeringscertifikatet har upphört" i avsnittet "Ett problem uppstod vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="5c6fa-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="5c6fa-107">Följ anvisningarna i [Uppdatera eller reparera inställningarna för en federerad domän i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="5c6fa-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="5c6fa-108">Mer information om hur du förnyar federationscertifikat finns [i Förnya federationscertifikat för Microsoft 365 och Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="5c6fa-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
