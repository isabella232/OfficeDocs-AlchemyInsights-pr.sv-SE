---
title: Lösenordsprinciper
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747054"
---
# <a name="password-policies"></a>Lösenordsprinciper

**Jag har problem med lösenordsprincipen för en användare**

- Lösenordsprincipen för en användare beror på om användaren endast är molnbaserad eller lokal.
- Endast användare i molnet måste välja ett lösenord som uppfyller kraven i den här artikeln: [Lösenordsprinciper som endast gäller för molnanvändarkonton](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokala användare måste välja ett lösenord som uppfyller de lokala kraven. Om en lokal användare inte kan ange sitt lösenord ska du kontrollera dina lokala krav.

**Jag vet inte hur jag anger eller kontrollerar förfalloprinciper för lösenord**

- Du kan ange och kontrollera förfalloprincipen för molnanvändare i klientorganisationen med hjälp av PowerShell. Följ anvisningarna i den här artikeln: [Ange eller kontrollera lösenordsprinciper med hjälp av PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Förfalloprincipen för lösenord för lokala användare anges i din lokala AD.

**Andra användbara länkar:**
- [Komma igång med återställning av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Felsöka administratörsinitierad lösenordsåterställning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
