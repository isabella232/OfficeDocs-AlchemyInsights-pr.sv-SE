---
title: En lokal Federation Service certifikat löper ut
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492106"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>En lokal Federation Service certifikat löper ut

Lös problemet så här:
  
- Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om den inte redan är installerat modulen). Genom att gå till [Azure Active Directory PowerShell för diagram](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Följ stegen i den ”Scenario 1: AD FS-token-signering certifikatet gått ut” avsnitt av [”Det gick inte att komma åt webbplatsen” fel från AD FS när en federerad användare loggar in på Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Följ stegen i t[hur du uppdaterar eller reparera inställningarna för en extern domän i Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Mer information om hur du förnyar certifikat Federation finns i [Förnya certifikat för O365 och Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

