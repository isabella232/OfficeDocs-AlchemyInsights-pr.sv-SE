---
title: 'AIP: principer fungerar inte som förväntat'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663207"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: principer fungerar inte som förväntat

Azure information Protection: principer fungerar inte som förväntat, se nedan för rekommenderade rikt linjer för olika princip problem:

1. Om du har problem med de visuella märkningarna kan du gå igenom [när de visuella märkningarna tillämpas](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Om du har problem med automatiska etiketter kan du läsa om [hur du konfigurerar villkoren för automatisk och Rekommenderad klassificering för Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och [vilken känslig information som kan](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)hämtas.
3. Om du har problem med inbyggt/pfile-skydd kan du läsa igenom [konfigurationen för fil-API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrol lera om du använder begränsade principer som inte har kon figurer ATS korrekt: [Konfigurera Azure information Protection policy för specifika användare med hjälp av begränsade principer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Om automatisk etikett inte fungerar för Outlook när du bifogar ett dokument med etiketter kontrollerar du att DRMEncryptProperty inte har definierats enligt beskrivningen här: [IRM-registerpostens inställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Om du fortfarande har problem kan du samla in Azure information Protection client-loggar och bifoga de exporterade loggarna till den här biljetten.

1. Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.
2. Klicka på **skydda/känslighets**  >  **Hjälp och feedback**.
3. Klicka på **Exportera loggar**.
4. Spara loggarna på valfri plats och bifoga dem till den här tjänst förfrågan.

Fler resurser:

- [Konfigurera en etikett för visuell märkning för Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Granska dokumentationen för Azure information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Använda känslighets etiketter i Microsoft 365-appar](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

