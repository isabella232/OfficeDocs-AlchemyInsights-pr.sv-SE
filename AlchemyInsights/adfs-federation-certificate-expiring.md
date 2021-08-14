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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952987"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation Certificate Expiring

Lös problemet genom att följa de här stegen:
  
1. Installera Microsoft Azure Active Directory för Windows PowerShell på datorn (om modulen inte redan är installerad). Det gör du genom att gå [till Hantera Azure AD med Windows PowerShell](https://aka.ms/aadposh).

2. Följ anvisningarna i avsnittet "Scenario 1: AD FS-token-signeringscertifikatet har upphört" i avsnittet "Ett problem uppstod vid åtkomst till webbplatsen" från AD FS när en federerad användare loggar in på Microsoft 365, Azure eller [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Följ anvisningarna i [Uppdatera eller reparera inställningarna för en federerad domän i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Mer information om hur du förnyar federationscertifikat finns [i Förnya federationscertifikat för Microsoft 365 och Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
