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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695197"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Att åtgärda Microsoft 365-apparna "din dators betrodda plattformsmodulen fungerar inte korrekt"

Lös problemet genom att prova med följande:

- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Rensa Office-uppgifter](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.<br/>
    **Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pröva [användar återställnings processen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) för att åtgärda fel i TPM (Trusted Platform Module).
- Ange EnableADAL = 0 så här:  
    1. Högerklicka på Start-knappen i Windows, Välj **Kör**, Skriv **regedit**och välj sedan **OK**.
    2. Välj **Ja** om du vill tillåta att Registereditorn gör ändringar på enheten.
    3. I Registereditorn lägger du till ett DWORD-värde för **EnableADAL** med en inställning på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Mer information finns i [anslutnings problem i Logga in efter uppdatering till Office 2016 version 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).