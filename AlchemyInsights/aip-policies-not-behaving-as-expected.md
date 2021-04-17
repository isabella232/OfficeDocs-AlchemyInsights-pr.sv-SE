---
title: 'AIP: Principer fungerar inte som förväntat'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821645"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Principer fungerar inte som förväntat

Azure Information Protection: Principer fungerar inte som förväntat. Se följande för rekommenderade riktlinjer för olika principproblem:

1. Om du har problem med visuella markeringar kan du läsa [När visuella markeringar används](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Om du har problem med automatisk märkning kan du läsa Konfigurera villkor för automatisk och rekommenderad klassificering för [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och Vilka typer av känslig information letar [efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Om du har problem med inbyggt/Pfilskydd kan du läsa File [API-konfiguration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollera om du använder omfattningsprinciper som inte är korrekt konfigurerade: Konfigurera Azure Information Protection-principen för specifika användare med hjälp av [omfattande principer.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Om automatisk märkning inte fungerar för Outlook när du bifogar ett etiketterat dokument kontrollerar du att DRMEncryptProperty inte har definierats enligt beskrivningen här: IRM-registerinställningar för [säkerhet.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Om du fortfarande har problem samlar du in Azure Information Protection-klientloggar och bifogar de exporterade loggarna i det här ärendeet.

1. Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.
2. Klicka **på Skydda/känslighet**  >  **Hjälp och feedback.**
3. Klicka **på Exportera loggar**.
4. Spara loggarna till ditt val av plats och bifoga dem till denna tjänstbegäran.

Fler resurser:

- [Konfigurera en etikett för visuella markeringar för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Granska dokumentationen för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Använda känslighetsetiketter i Microsoft 365-appar](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

