---
title: Distribuera Office 365 ProPlus för delad användning på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959477"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Office 365 ProPlus för delad användning på RDS, Terminal Server eller VDI

Så här distribuerar du Office 365 ProPlus med Remote Desktop Services (RDS), tidigare namngivna Terminal Services:
- Du måste ha en Microsoft 365 för affärsplan eller en Office 365-plan som innehåller Office 365 ProPlus, till exempel Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE] 
   > Office 365 Business och Office 365 Business Premium-abonnemang innehåller inte Office 365 ProPlus.
- Du måste aktivera [delad datoraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan också hämta och köra [Microsoft support och återställning assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Office 365 ProPlus i läget för delad datoraktivering.

Mer information om förutsättningar, installationsanvisningar och vägledning om anpassade installationer med hjälp av Office Deployment Tool finns i [distribuera office 365 ProPlus med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Så här åtgärdar du fel som rör delad datoraktivering:
- Se [Felsöka problem med aktivering av delade datorer för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [återställa aktiveringstillståndet för Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Om du vill installera Office 365 ProPlus på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, använder du följande steg:

1.  Kontrollera vad Office 365 plan du har. [Läs mer](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Om det behövs växlar du till en annan Office 365-plan. [Läs mer](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Om Office redan är installerat på RDS-servern med andra Office 365-abonnemang avinstallerar du det. Till exempel, genom att gå till **Kontrollpanelen** > **Avinstallera ett program**. Avinstallera med hjälp av [Microsoft support och Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du kör i problem.
4.  På RDS-servern loggar du in på Microsoft 365 administratörscenter med ditt administratörskonto och [installerar Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  När Office har installerats ska ***du inte öppna eller logga in*** på några Office-program.
6.  Aktivera delad datoraktivering genom att redigera registret på RDS-servern genom att följa dessa steg:
   1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**. Skriv **regedit**i rutan Öppna och välj sedan **OK**.
   2. Välj **Ja** när du tillfrågas om du vill tillåta att Registereditorn gör ändringar på enheten.
   3. I Registereditorn lägger du till ett strängvärde för **Sharedcomputerlicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \Software\microsoft \Office\ClickToRun\Configuration.
   4. ***Logga in som en slutanvändare*** på RDS-servern och [Kontrollera att aktivering av delade datorer är aktiverat för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

