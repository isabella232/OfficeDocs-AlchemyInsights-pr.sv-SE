---
title: Distribuera Microsoft 365-program för företag för delad användning i RDS, Terminal Server eller VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200691"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Microsoft 365-program för företag för delad användning i RDS, Terminal Server eller VDI

Så här distribuerar du Microsoft 365-appar för företag med Fjärrskrivbordstjänster (RDS) som tidigare hette Terminal Services:

- Du måste ha ett Microsoft 365 för företag-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise, E3 eller Enterprise E5.
   > [!NOTE]
   > Microsoft 365-programmen för företag och Microsoft 365 Business Standard-abonnemangen innehåller inte Microsoft 365-appar för företag.
- Du måste aktivera [aktivering på delad dator.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Du kan också ladda ned och köra [Microsoft Support- och](https://aka.ms/SaRA_OfficeSCA_M365Portal) återställningsassistenten för att installera Microsoft 365-appar för företag i läget för aktivering på delad dator.

Mer information om krav, installationsanvisningar och vägledning för anpassade installationer med hjälp av distributionsverktyget för Office finns i Distribuera [Microsoft 365-program](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)för företag med hjälp av Fjärrskrivbordstjänster.

Så här åtgärdar du fel som rör aktivering av delad dator:

- Se [Felsöka problem med aktivering av delad dator för Microsoft 365-program för företag.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).

Om du vill installera Microsoft 365-appar för företag på RDS från administrationscentret för Microsoft 365 ***med*** standardinstallationsinställningarna gör du så här:

1. Kontrollera vilken prenumeration du har. [Läs mer](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Byt till en annan prenumeration om det behövs. [Läs mer](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Om Office redan är installerat på RDS-servern med några andra Microsoft-prenumerationer avinstallerar du det. Genom att till exempel gå till **Kontrollpanelen Avinstallera**  >  **ett program**. Avinstallera med [Microsoft Support- och återställningsassistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du har problem.
4. På RDS-servern loggar du in på administrationscentret för Microsoft 365 med ditt administratörskonto och installerar [Microsoft 365-program för företag.](https://portal.office.com/OLS/MySoftware.aspx)
5. När Office har installerats ***ska du inte öppna eller logga in i*** något Office-program.
6. Aktivera aktivering av delad dator på RDS-servern genom att redigera registret så här:
   1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**. Skriv regedit i rutan **Öppna** klicka sedan på **OK**.
   2. Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.
   3. I Registereditorn lägger du till strängvärdet **SharedComputerLicensing** med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logga ***in*** som slutanvändare på RDS-servern och kontrollera att aktivering av delade datorer är aktiverat för [Microsoft 365-appar för företag.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
