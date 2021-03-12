---
title: Problem med att logga in på Microsoft 365-appar
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709124"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Åtgärda meddelandet "Din dators modul för betrodd plattform fungerar inte korrekt" i Microsoft 365-programmen

Lös problemet genom att prova med följande:

- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) med Hjälp av Autentiseringshanteraren.<br/>
    **Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0. (Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Prova [återställningsprocessen för användare för](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) att åtgärda TPM-fel (Trusted Platform Module).
- Ställ in EnableADAL = 0 så här:  
    1. Högerklicka på Start-knappen i Windows, välj **Kör,** skriv **regedit** och välj sedan **OK.**
    2. Välj **Ja** om du vill tillåta registereditorn att göra ändringar på din enhet.
    3. Lägg till ett DWORD-värde för **EnableADAL** i Registereditorn med inställningen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Mer information finns i Anslutningsproblem vid inloggning efter uppdatering till [Office 2016 version 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)