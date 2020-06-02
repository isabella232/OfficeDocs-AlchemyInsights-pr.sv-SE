---
title: 'AIP: Principer som inte beter sig som förväntat'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506576"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Principer som inte beter sig som förväntat

Azure Information Protection: Principer som inte fungerar som förväntat, se följande för rekommenderade riktlinjer för olika principproblem:

1. Om du har problem med visuella markeringar läser du [När visuella markeringar används](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Om du har problem med automatisk märkning läser du Så här konfigurerar du [villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och Vilka känsliga [informationstyper som letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Om du har problem med Native/Pfile-skydd läser du [fil-API-konfigurationen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollera om du använder begränsade principer som inte är korrekt konfigurerade: [Så här konfigurerar du Azure-informationsskyddsprincipen för specifika användare med hjälp av scoped-principer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Om automatisk märkning inte fungerar för Outlook när du bifogar ett märkt dokument kontrollerar du att DRMEncryptProperty inte definieras som beskrivet här: [IRM-registerinställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Om du fortfarande har problem samlar du in Azure Information Protection-klientloggar och bifogar de exporterade loggarna till den här biljetten.

1. Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.
2. Klicka på Hjälp och feedback **om skydd/känslighet**  >  **Help and feedback**.
3. Klicka på **Exportera loggar**.
4. Spara loggarna till ditt val av plats och bifoga dem till den här servicebegäran.

Fler resurser:

- [Konfigurera en etikett för visuella markeringar för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Granska Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Använda känslighetsetiketter i Office-appar](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

