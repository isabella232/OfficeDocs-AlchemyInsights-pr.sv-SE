---
title: Distribuera Microsoft 365-appar för företag för delad användning i RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325621"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Microsoft 365-appar för företag för delad användning i RDS, Terminal Server eller VDI

Så här distribuerar Microsoft 365-appar för företag du med Fjärrskrivbordstjänster (RDS) som tidigare hette Terminal Services:

- Du måste ha ett Microsoft 365 för företag-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365-appar för företag, till exempel E3 Office 365 Enterprise Enterprise E5.
   **Obs!** Microsoft 365-applikationer för affärsverksamhet och Microsoft 365 Business Standard ingår inte i Microsoft 365-appar för företag.
- Du måste aktivera [aktivering på delad dator.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Obs!** Du kan också ladda ned och köra [Microsoft-Support- och återställningsassistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) installera Microsoft 365-appar för företag i aktiveringsläge för delad dator.

Mer information om krav, installationsanvisningar och vägledning för anpassade installationer med hjälp av distributionsverktyget för Office finns i Distribuera Microsoft 365-appar för företag med hjälp av [Fjärrskrivbordstjänster.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Så här åtgärdar du fel som rör aktivering av delad dator:

- Se [Felsöka problem med aktivering av delad dator för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).

Om du vill installera Microsoft 365-appar för företag RDS från Administrationscenter för Microsoft 365, ***som använder standardinställningarna*** för installation, gör du så här:

1. Kontrollera vilken prenumeration du har. [Läs mer](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Byt till en annan prenumeration om det behövs. [Läs mer](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Om Office rds-servern som använder andra Microsoft-prenumerationer avinstallerar du den. Genom att till exempel gå till **Kontrollpanelen Avinstallera**  >  **ett program**. Avinstallera med [Microsoft Support- och återställningsassistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du får problem.
4. På RDS-servern loggar du in på Administrationscenter för Microsoft 365 administratörskontot och [installerar Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).
5. När Office är installerat ***ska du inte öppna eller logga in i*** något Office program.
6. Aktivera aktivering av delad dator på RDS-servern genom att redigera registret så här:
   1. Högerklicka på Windows längst ned till vänster på skärmen och välj **Kör.** Skriv regedit i rutan **Öppna** klicka sedan på **OK**.
   2. Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.
   3. I Registereditorn lägger du till strängvärdet **SharedComputerLicensing** med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logga in som slutanvändare på ***RDS-servern och kontrollera*** att [aktivering av delad dator är aktiverad för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
