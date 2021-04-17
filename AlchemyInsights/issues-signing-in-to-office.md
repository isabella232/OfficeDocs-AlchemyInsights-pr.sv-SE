---
title: Problem med inloggning på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833057"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom inloggningsskärm i Microsoft 365-appar

Prova följande för att åtgärda problemet:
- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Återställ Internet Explorer-alternativ: Gå till Verktyg   >  **Internetalternativ**  >  **Avancerade**  >  **återställningsinställningar** för Internet Explorer (observera att du förlorar anpassade inställningar) och försök sedan logga in på Office igen.
- Inaktivera Windows Defender Application Guard (WDAG) eller liknande brandvägg eller antivirusprogram:
    1. I Kontrollpanelen går du till **Program** och väljer sedan **Aktivera eller inaktivera Windows-funktioner.**
    2. Om Windows Defender Application Guard är aktiverat provar du att inaktivera det.<br/>
    **Obs!** Du kan behöva starta om datorn.
- Kontrollera att plugin-programmet Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av något program eller brandvägg/antivirusprogram.
- [Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows Autentiseringshanteraren.<br/>
    **Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0. (Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)

Mer information finns i Anslutningsproblem vid inloggning efter uppdatering till [Office 2016 version 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)