---
title: Problem med att logga in i Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695305"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tom inloggnings skärm i Microsoft 365-appar

Lös problemet genom att pröva följande:
- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Återställ alternativen för Internet Explorer: gå **till**  >  **Internet alternativ**  >  **avancerade**  >  **Återställ inställningar för Internet Explorer** (Observera att du kommer att förlora anpassade inställningar) och försök sedan att logga in på Office igen.
- Inaktivera Windows Defender Application Guard (WDAG) eller liknande brand vägg eller antivirus program:
    1. Gå till **program**på kontroll panelen och välj **Aktivera eller inaktivera Windows-funktioner**.
    2. Om Windows Defender Application Guard är aktiverat kan du försöka med att inaktivera det.<br/>
    **Obs!** Du kan behöva starta om datorn.
- Kontrol lera att plugin-programmet Microsoft. AAD. BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av något program eller brand vägg/antivirus program.
- [Rensa Office-uppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.<br/>
    **Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Mer information finns i [anslutnings problem i Logga in efter uppdatering till Office 2016 version 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).