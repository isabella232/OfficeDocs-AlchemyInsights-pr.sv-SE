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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737207"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-Federationscertifikat upphör att gälla

Lös problemet så här:
  
1. Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad). Genom att gå till [Hantera Azure AD med hjälp av Windows PowerShell](https://aka.ms/aadposh).

2. Följ stegen i "Scenario 1: AD FS-tokensignering certifikatet har upphört att gälla" avsnittet ["Det gick inte att komma åt webbplatsen" fel från AD FS när en federerad användare loggar in på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Följ stegen i [Uppdatera eller reparera inställningarna för en federerad domän i Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Mer information om hur du förnyar Federations certifikat finns i [förnya Federations certifikat för Office 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
