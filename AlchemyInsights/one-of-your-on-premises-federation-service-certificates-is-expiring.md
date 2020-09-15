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
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Ett av dina lokala Federations tjänst certifikat upphör att gälla

Lös problemet genom att följa de här stegen:
  
- Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad). För att göra det går du till [Azure Active Directory PowerShell för Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Följ anvisningarna i "Scenario 1: certifikatet för token-signerings certifikat för AD FS upphörde att gälla" i ["det uppstod ett problem vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Följ anvisningarna i så här [uppdaterar eller reparerar du inställningarna för en federerad domän i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Mer information om hur du förnyar Federations certifikat finns i [certifikat förnyelse för O365 och Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

