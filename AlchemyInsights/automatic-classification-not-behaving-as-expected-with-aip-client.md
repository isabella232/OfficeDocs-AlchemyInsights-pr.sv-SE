---
title: Automatisk klassificering fungerar inte som förväntat med AIP-klienten
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508394"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassificering fungerar inte som förväntat med AIP-klienten

Automatisk klassificering fungerar inte som förväntat, använd följande rekommenderade riktlinjer:

1. Om du har problem med automatisk märkning läser du Så här konfigurerar du [villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) och Vilka känsliga [informationstyper som letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontrollera om du använder begränsade principer som inte är korrekt konfigurerade: [Så här konfigurerar du Azure-informationsskyddsprincipen för specifika användare med hjälp av scoped-principer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Om automatisk märkning inte fungerar för Outlook när du bifogar ett märkt dokument kontrollerar du att det `DRMEncryptProperty` inte definieras som beskrivs här: [IRM-registerinställningar för säkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Om du har använt de [inbyggda informationstyperna](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) för din Azure Information Protection-princip kontrollerar du att ditt innehåll matchar det förväntade formatet.
5. Kontrollera att etiketten är korrekt konfigurerad för **Automatisk** eller **Rekommenderad**. (**Automatisk** märkning är tillgänglig för alla Office-appar, medan **Rekommenderas** är tillgängligt för alla Office-appar utom Outlook.)
6. Du kan inte använda automatisk klassificering för dokument och e-postmeddelanden som tidigare har märkts manuellt eller tidigare automatiskt märkts med en högre klassificering.  Mer information finns i: [Hur automatiska eller rekommenderade etiketter används](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Om du fortfarande har problem samlar du in Azure Information Protection-klientloggar och bifogar de exporterade loggarna till din supportbiljett. Så här exporterar du Azure Information Protection-loggar:
    - Öppna ett Office-dokument eller skapa ett nytt e-postmeddelande i Outlook.
    - Klicka på Hjälp och feedback **om skydd/känslighet**  >  **Help and feedback**.
    - Klicka på **Exportera loggar**.
    - Spara loggarna till ditt val av plats och bifoga dem till din servicebegäran.

Mer information finns i:

- [Konfigurera villkor för automatisk och rekommenderad klassificering för Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Hjälpguider för vanliga scenarier som använder Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Granska Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Granska Prenumerationer och funktioner för Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav för Azure-informationsskydd](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Snabbstartshandledning för Azure-informationsskydd](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Ladda ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
