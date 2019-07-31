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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938360"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Fastställande av meddelandet ”datorns betrodda Platform module inte fungerar som det ska” apps Office

Försök med följande om du vill åtgärda det här felet:

- Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.<br/>
    **Observera:** Registersökvägar 2016 för Office har ändrats till 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Försök åtgärda fel Trusted Platform Module (TPM) [användaren återställningsprocessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .
- Ange EnableADAL = 0 med hjälp av följande steg:  
    1. Högerklicka på Start, Välj **Kör**, Skriv **regedit**och klicka sedan på **OK**.
    2. Välj **Ja** så att Registereditorn för att göra ändringar i din enhet.
    3. I Registereditorn kan du lägga till DWORD-värdet **EnableADAL** med en inställning på **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Mer information finns i [anslutning problem i logga in efter uppdatering till Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).