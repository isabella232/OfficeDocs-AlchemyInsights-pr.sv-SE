---
title: Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704723"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI

Så här distribuerar du Microsoft 365-appar för företag med fjärrskrivbordstjänster (RDS), tidigare Terminal Services:
- Du måste ha ett Microsoft 365 For Business-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365 Apps för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 Apps for business och Microsoft 365 Business Premium Standard-abonnemangen innehåller inte Microsoft 365 Apps för företag.
- Du måste aktivera [aktivering av delad dator](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan också hämta och köra [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365 Apps för företag i aktiveringsläge för delade datorer.

Mer information om förutsättningar, installationsinstruktioner och vägledning om anpassade installationer med hjälp av Distributionsverktyget för Office finns i [Distribuera Microsoft 365-appar för företag med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Så här åtgärdar du fel relaterade till aktivering av delade datorer:
- Se [Felsöka problem med aktivering av delade datorer för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).

Om du vill installera Microsoft 365 Apps för företag på RDS från Microsoft 365 admin center, ***som använder standardinstallationsinställningar,*** gör du så här:

1.    Kontrollera vilken prenumeration du har. [Läs mer](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Om det behövs växlar du till en annan prenumeration. [Läs mer](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Om Office redan är installerat på RDS-servern med andra Microsoft-prenumerationer avinstallerar du det. Till exempel genom att gå till **Kontrollpanelen** > **Avinstallera ett program**. Avinstallera med Hjälp av [Microsoft Support och Återställningsassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du har problem.
4.    Logga in på Microsoft 365-administrationscentret med administratörskontot på RDS-servern och [installera Microsoft 365 Apps för företag](https://portal.office.com/OLS/MySoftware.aspx).
5.    När Office har ***installerats ska du inte öppna eller logga in på*** några Office-program.
6.    Aktivera delad datoraktivering på RDS-servern genom att redigera registret genom att följa dessa steg:
   1. Högerklicka på Windows-knappen längst ned till vänster på skärmen och välj **Kör**. Skriv **regedit**i rutan Öppna och välj sedan **OK**.
   2. Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.
   3. Lägg till ett strängvärde för **SharedComputerLicensing** i Registereditorn med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logga in som ***slutanvändare på*** RDS-servern och [kontrollera att aktivering av delad dator är aktiverad för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

