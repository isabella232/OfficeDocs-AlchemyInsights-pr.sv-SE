---
title: Installera Office på en terminalserver – ej licensierad
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322017"
---
# <a name="installing-office-on-a-terminal-server"></a>Installera Office på en terminalserver

För distribution Microsoft 365-appar för företag på en Windows Server med Fjärrskrivbordstjänster (RDS), som tidigare hette Terminal Services:
  
- Du måste ha ett Microsoft 365-abonnemang som omfattar Microsoft 365-appar för företag, till exempel E3 Office 365 Enterprise Enterprise E5. I Microsoft 365-applikationer för affärsverksamhet och Microsoft 365-applikationer för affärsverksamhet Premium ingår inte några Microsoft 365-appar för företag.

- Du måste aktivera aktivering [på delad dator.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Om du vill installera Microsoft 365-appar för företag RDS från Administrationscenter för Microsoft 365, som använder standardinställningarna för ***installation,*** gör du följande.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Kontrollera vilken Microsoft 365 du har. [Lär dig hur](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Om det behövs byter du till en annan Microsoft 365 prenumeration. [Lär dig hur](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Om Office har installerats på RDS-servern med andra prenumerationer Microsoft 365 avinstallerar du den. Genom att till exempel gå till Kontrollpanelen Avinstallera \> ett program. Avinstallera med [Microsoft Support- och återställningsassistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du får problem.

4. På RDS-servern loggar du in på Administrationscenter för Microsoft 365 administratörskonto och [installerar Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).

5. När Office har ***installerats ska du inte öppna eller logga in*** i något Office program.

6. Aktivera aktivering av delad dator på RDS-servern genom att redigera registret så här:

1. Högerklicka på Windows i det nedre vänstra hörnet av skärmen och välj Kör. Skriv **regedit i rutan Öppna** och välj sedan OK.

2. Välj Ja när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.

3. I Registereditorn lägger du till strängvärdet **SharedComputerLicensing** med inställningen 1 under \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Logga in som slutanvändare på ***RDS-servern och kontrollera*** att [aktivering av delad dator är aktiverad för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Mer information om krav, installationsanvisningar och vägledning för anpassade installationer med hjälp av distributionsverktyget för Office finns i Distribuera Microsoft 365-appar för företag med hjälp av [Fjärrskrivbordstjänster.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Information om hur du åtgärdar fel som rör aktivering av delad dator finns i [Felsöka problem med aktivering av delad dator Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  