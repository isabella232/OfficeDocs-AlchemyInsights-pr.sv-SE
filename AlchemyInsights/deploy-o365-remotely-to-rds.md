---
title: Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745553"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI

Så här distribuerar du Microsoft 365-appar för företag med fjärr skrivbords tjänster (RDS), tidigare namngivna Terminal Services:
- Du måste ha ett Microsoft 365 för företag-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Microsoft 365-apparna för företag och Microsoft 365 Business Premium standard-abonnemang inkluderar inte Microsoft 365-appar för företag.
- Du måste aktivera [delad dator aktivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan också ladda ned och köra [Microsoft-assistenten för support och återställning](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365-appar för företag i aktiverings läget för delad dator.

Mer information om förutsättningar, konfigurations instruktioner och vägledning om anpassade installationer med hjälp av distributions verktyget för Office finns i [distribuera Microsoft 365-appar för företag med hjälp av fjärr skrivbords tjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Så här löser du problem med att aktivera en delad dator:
- Se [Felsöka problem med att aktivera delad dator för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).

Om du vill installera Microsoft 365-appar för företag på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, gör du så här:

1.    Kontrol lera vilken prenumeration du har. [Läs mer](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Byt eventuellt till ett annat abonnemang. [Läs mer](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Om Office redan är installerat på RDS-servern med andra Microsoft-abonnemang avinstallerar du det. Till exempel genom att gå till **kontroll panelen**  >  **Avinstallera ett program**. Avinstallera med [Microsoft support-och återställnings assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du stöter på problem.
4.    Logga in på administrations centret för Microsoft 365 med ditt administratörs konto och [Installera Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).
5.    När Office är installerat kan du ***inte öppna eller logga*** in på något Office-program.
6.    Aktivera delad dator aktivering på RDS-servern genom att redigera registret genom att följa de här stegen:
   1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**. I rutan Öppna skriver du **regedit**och väljer sedan **OK**.
   2. Välj **Ja** när du uppmanas att tillåta att Registereditorn gör ändringar på enheten.
   3. I Registereditorn lägger du till ett sträng värde för **SharedComputerLicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. ***Logga in som slutanvändare*** på RDS-servern och [kontrol lera att aktivera delad dator är aktiverat för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

