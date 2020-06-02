---
title: Installera kontor på en Terminal Server - Olicensierad
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508646"
---
# <a name="installing-office-on-a-terminal-server"></a>Installera Office på en Terminal Server

För distribution av Microsoft 365-appar för företag på en Windows Server med fjärrskrivbordstjänster ( RDS), tidigare terminaltjänster:
  
- Du måste ha en Microsoft 365-prenumeration som innehåller Microsoft 365 Apps för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5. Microsoft 365 Apps for business och Microsoft 365 Apps for business Premium-abonnemang innehåller inte Microsoft 365 Apps för företag.

- Du måste aktivera [aktivering av delad dator](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Om du vill installera Microsoft 365 Apps for enterprise på RDS från Microsoft 365 admin center, ***som använder standardinstallationsinställningar,*** gör du så här.

> [!TIP]
> Du kan också hämta och köra [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365 Apps för företag i aktiveringsläge för delade datorer.
  
1. Kontrollera vilken Microsoft 365-prenumeration du har. [Lära sig](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Om det behövs växlar du till en annan Microsoft 365-prenumeration. [Lära sig](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Om Office redan är installerat på RDS-servern med andra Microsoft 365-prenumerationer avinstallerar du det. Till exempel genom att gå till Kontrollpanelen \> Avinstallera ett program. Avinstallera med Hjälp av [Microsoft Support och Återställningsassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du har problem.

4. Logga in på Microsoft 365-administrationscentret med administratörskontot på RDS-servern och [installera Microsoft 365 Apps för företag](https://portal.office.com/OLS/MySoftware.aspx).

5. När Office har ***installerats ska du inte öppna eller logga in på*** några Office-program.

6. Aktivera delad datoraktivering på RDS-servern genom att redigera registret genom att följa dessa steg:

1. Högerklicka på Windows-knappen i det nedre vänstra hörnet på skärmen och välj Kör. Skriv **regedit**i rutan Öppna och välj sedan OK.

2. Välj Ja när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.

3. Lägg till ett strängvärde för **SharedComputerLicensing** i Registereditorn med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Logga in som ***slutanvändare på*** RDS-servern och [kontrollera att aktivering av delad dator är aktiverad för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Mer information om förutsättningar, installationsinstruktioner och vägledning om anpassade installationer med hjälp av Distributionsverktyget för Office finns i [Distribuera Microsoft 365-appar för företag med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Information om hur du åtgärdar fel i samband med aktivering av delad dator finns [i Felsöka problem med aktivering av delad dator för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  