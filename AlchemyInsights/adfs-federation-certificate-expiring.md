---
title: AD FS-Federation certifikatet upphör att gälla
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
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357983"
---
# <a name="adfs-federation-certificate-expiring"></a>AD FS-Federation certifikatet upphör att gälla

Lös problemet så här:
  
1. Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om den inte redan är installerat modulen). Gör detta genom att gå till [Hantera Azure AD med hjälp av Windows PowerShell](https://aka.ms/aadposh).

2. Följ stegen i den ”Scenario 1: AD FS-token-signering certifikatet gått ut” avsnitt av [”Det gick inte att komma åt webbplatsen” fel från AD FS när en federerad användare loggar in på Office 365, Azure, eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Följ instruktionerna i [hur du uppdaterar eller reparera inställningarna för en extern domän i Office 365, Azure, eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Mer information om hur du förnyar certifikat Federation finns i [Förnya federationstjänstens certifikat för Office 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
