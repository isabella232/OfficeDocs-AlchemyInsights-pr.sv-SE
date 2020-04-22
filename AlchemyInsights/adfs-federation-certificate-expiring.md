---
title: ADFS Federation-certifikatet löper ut
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710425"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation-certifikatet löper ut

Så här löser du problemet:
  
1. Installera Microsoft Azure Active Directory Module för Windows PowerShell på datorn (om modulen inte redan är installerad). Det gör du genom att gå till [Hantera Azure AD med Windows PowerShell](https://aka.ms/aadposh).

2. Följ stegen i avsnittet "Scenario 1: AD FS-tokensigneringscertifikatet har upphört att gälla" i [felet "Det uppstod ett problem med att komma åt webbplatsen" från AD FS när en federerad användare loggar in på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Följ stegen i [Uppdatera eller reparera inställningarna för en federerad domän i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Mer information om hur du förnyar federationscertifikat finns i [Förnya federationscertifikat för Microsoft 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
