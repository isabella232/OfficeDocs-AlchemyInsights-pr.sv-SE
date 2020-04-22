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
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761401"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Ett av dina lokala federationsservicecertifikat löper ut

Så här löser du problemet:
  
- Installera Microsoft Azure Active Directory Module för Windows PowerShell på datorn (om modulen inte redan är installerad). Det gör du genom att gå till [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Följ stegen i avsnittet "Scenario 1: AD FS-tokensigneringscertifikatet har upphört att gälla" i [felet "Det uppstod ett problem med att komma åt webbplatsen" från AD FS när en federerad användare loggar in på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Följ stegen i t[Så här uppdaterar eller reparerar du inställningarna för en federerad domän i Office 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Mer information om hur du förnyar federationscertifikat finns i [Förnyelse av certifikat för O365 och Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

