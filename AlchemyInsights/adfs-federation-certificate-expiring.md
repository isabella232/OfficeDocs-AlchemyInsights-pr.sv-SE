---
title: Certifikat för ADFS-federationen upphör
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686771"
---
# <a name="adfs-federation-certificate-expiring"></a>Certifikat för ADFS-federationen upphör

Lös problemet genom att följa de här stegen:
  
1. Installera Microsoft Azure Active Directory-modulen för Windows PowerShell på datorn (om modulen inte redan är installerad). För att göra det går du till [Hantera Azure AD via Windows PowerShell](https://aka.ms/aadposh).

2. Följ anvisningarna i "Scenario 1: certifikatet för token-signerings certifikat för AD FS upphörde att gälla" i ["det uppstod ett problem vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Följ stegen i [Uppdatera eller reparera inställningarna för en federerad domän i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Mer information om hur du förnyar Federations certifikat finns i [förnya Federations certifikat för Microsoft 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
