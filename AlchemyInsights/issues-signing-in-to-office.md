---
title: Problem att logga in på Office apps
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938359"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tom inloggningsskärmen i Office apps

Om du vill åtgärda det här problemet kan du prova följande:
- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Återställ Internet Explorer-alternativ: Gå till **Verktyg** > **Internet-alternativ** > **Avancerat** > **Återställ inställningar för Internet Explorer** (Observera att du kommer att förlora anpassade inställningar) och försök sedan logga in på Office igen.
- Inaktivera Windows Defender programmet Guard (WDAG) eller något liknande brandvägg eller anti-virus program:
    1. Gå till **program**på Kontrollpanelen och klicka på **Aktivera Windows-funktioner på eller av**.
    2. Om Windows Defender programmet Guard är aktiverad kan du prova att inaktivera den.<br/>
    **Observera:** Du kan behöva starta om datorn.
- Se till att Microsoft.AAD.BrokerPlugin [Ledsagardokumentet WAM plugin-program](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av ett program eller en brandvägg/mot-virus program.
- [Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.<br/>
    **Observera:** Registersökvägar 2016 för Office har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Mer information finns i [anslutning problem i logga in efter uppdatering till Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).