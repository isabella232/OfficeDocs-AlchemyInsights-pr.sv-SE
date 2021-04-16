---
title: Ett av dina lokala federationstjänstcertifikat går ut
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810070"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Ett av dina lokala federationstjänstcertifikat går ut

Lös problemet genom att följa de här stegen:
  
- Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad). Det gör du genom att gå [till Azure Active Directory PowerShell för Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Följ anvisningarna i avsnittet "Scenario 1: AD FS-token-signeringscertifikatet har upphört" i avsnittet "Ett problem uppstod vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Följ anvisningarna i Uppdatera eller reparera inställningarna för en [federerad domän i Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Mer information om hur du förnyar federationscertifikat finns i [Certifikatet förnyas för O365 och Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

