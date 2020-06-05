---
title: Problem med att logga in på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579919"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom inloggningsskärm i Microsoft 365-appar

Försök med följande om du vill åtgärda problemet:
- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Återställ Internet Explorer-alternativ: Gå till **Verktyg**  >  **Internet-alternativ**  >  **Avancerade**  >  **återställningsinställningar för Internet Explorer** (observera att du kommer att förlora anpassade inställningar) och försök sedan logga in på Office igen.
- Inaktivera Windows Defender Application Guard (WDAG) eller liknande brandväggs- eller antivirusprogram:
    1. Gå till Program **på**Kontrollpanelen och välj sedan **Aktivera eller inaktivera Windows-funktioner.**
    2. Om Windows Defender Application Guard är aktiverat kan du prova att inaktivera den.<br/>
    **Anm.:** Du kan behöva starta om datorn.
- Kontrollera att plugin-programmet Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av något program eller ett antivirusprogram för brandväggar/antivirusprogram.
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br/>
    **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. (T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)

Mer information finns [i Anslutningsproblem i inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).