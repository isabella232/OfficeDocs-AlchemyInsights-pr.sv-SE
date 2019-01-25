---
title: AD FS-Federation certifikatet upphör att gälla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492478"
---
# <a name="adfs-federation-certificate-expiring"></a>AD FS-Federation certifikatet upphör att gälla

Lös problemet så här:
  
1. Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om den inte redan är installerat modulen). Gör detta genom att gå till [Hantera Azure AD med hjälp av Windows PowerShell](https://aka.ms/aadposh).
    
2. Följ stegen i den ”Scenario 1: AD FS-token-signering certifikatet gått ut” avsnitt av [”Det gick inte att komma åt webbplatsen” fel från AD FS när en federerad användare loggar in på Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Följ instruktionerna i [hur du uppdaterar eller reparera inställningarna för en extern domän i Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Mer information om hur du förnyar certifikat Federation finns i [Förnya federationstjänstens certifikat för Office 365 och Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

