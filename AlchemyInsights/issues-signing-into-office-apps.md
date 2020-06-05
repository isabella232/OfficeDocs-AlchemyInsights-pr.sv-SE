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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579883"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Åtgärda microsoft 365-apparna "Datorns modul för betrodd plattform fungerar inte som den ska"

Lös problemet genom att prova med följande:

- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.<br/>
    **Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0. (T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)
- Prova [att återställa användaren för](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) att åtgärda TPM-fel (Trusted Platform Module).
- Ställ in EnableADAL = 0 med hjälp av följande steg:  
    1. Högerklicka på Start-knappen i Windows, välj **Kör**, skriv **regedit**och välj sedan **OK**.
    2. Välj **Ja** om du vill att Registereditorn ska kunna göra ändringar på enheten.
    3. I Registereditorn lägger du till ett DWORD-värde **för EnableADAL** med inställningen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Mer information finns [i Anslutningsproblem i inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).