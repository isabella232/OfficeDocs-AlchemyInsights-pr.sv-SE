---
title: Automatisk klassificering beter sig inte som förväntat med AIP-klienten
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979727"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassificering beter sig inte som förväntat med AIP-klienten

Använd följande rekommenderade riktlinjer om automatisk klassificering inte fungerar som förväntat:

1. Om du har problem med automatisk etikettering kan du gå till [Så här konfigurerar du villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och [Vad typerna av känslig information letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontrollera om du använder omfattningsprinciper som inte är korrekt konfigurerade: [Så här konfigurerar du Azure Information Protection-principen för specifika användare med hjälp av omfattningsprinciper](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Om automatisk etikettering inte fungerar för Outlook när du bifogar ett etiketterat dokument kontrollerar du att `DRMEncryptProperty` inte definierats enligt beskrivningen här: [IRM-registerinställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Om du har använt [inbyggda informationstyper](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) för Azure Information Protection-principen kontrollerar du att innehållet matchar det förväntade formatet.
5. Verifiera att etiketten är korrekt konfigurerad för **Automatisk** eller **Rekommenderad**. (**Automatisk** etikettering är tillgänglig för alla Microsoft 365-appar, medan den **rekommenderade** är tillgänglig för alla Microsoft 365-program förutom Outlook.)
6. Du kan inte använda automatisk klassificering för dokument och e-postmeddelanden som tidigare etiketterats manuellt eller tidigare etiketterats med en högre klassificering.  Mer information finns i: [Hur automatiska och rekommenderade etiketter används](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Om du fortfarande har problem kan du samla in Azure Information Protection-klientloggar och bifoga de exporterade loggarna i supportbegäran. För att exportera Azure Information Protection-loggar:
    - Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.
    - Klicka på **Skydda/Känslighet** > **Hjälp och feedback**.
    - Klicka på **Exportera loggar**.
    - Spara loggarna till platsen du valt och bifoga dem till din tjänstbegäran.

Mer information finns i:

- [Hur du kan konfigurera villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guider för vanliga scenarier där Azure Information Protection används](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Granska dokumentation om Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Granska prenumerationer och funktioner för Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Snabbstartskurs för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).
- [Hämta Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
