---
title: Installera Office på en terminalserver-olicensierad
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735407"
---
# <a name="installing-office-on-a-terminal-server"></a>Installera Office på en terminalserver

För distribution av Office 365 ProPlus på en Windows-Server med hjälp av Remote Desktop Services (RDS), tidigare namngivna Terminal Services:
  
- Du måste ha en Office 365-plan som innehåller Office 365 ProPlus, till exempel Office 365 Enterprise E3 eller Enterprise E5. Office 365 Business och Office 365 Business Premium-abonnemang innehåller inte Office 365 ProPlus.

- Du måste aktivera [delad datoraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Om du vill installera Office 365 ProPlus på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, så här:
  
1. Kontrollera vad Office 365 plan du har. [Lära sig](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Om det behövs växlar du till en annan Office 365-plan. [Lära sig](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Om Office redan är installerat på RDS-servern med andra Office 365-abonnemang avinstallerar du det. Till exempel, genom att gå till kontroll \> panelen Avinstallera ett program. Avinstallera med hjälp av [Microsoft support och Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du kör i problem.

4. På RDS-servern loggar du in på Microsoft 365 administratörscenter med ditt administratörskonto och [installerar Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. När Office har installerats ska ***du inte öppna eller logga in*** på några Office-program.

6. Aktivera delad datoraktivering genom att redigera registret på RDS-servern genom att följa dessa steg:

1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj Kör. Skriv **regedit**i rutan Öppna och välj sedan OK.

2. Välj Ja när du tillfrågas om du vill tillåta att Registereditorn gör ändringar på enheten.

3. I Registereditorn lägger du till ett strängvärde för **Sharedcomputerlicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. ***Logga in som en slutanvändare*** på RDS-servern och [Kontrollera att aktivering av delade datorer är aktiverat för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Mer information om förutsättningar, installationsanvisningar och vägledning om anpassade installationer med hjälp av Office Deployment Tool finns i [distribuera office 365 ProPlus med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Om du vill åtgärda fel i samband med aktivering av delade datorer läser du [Felsöka problem med aktivering av delade datorer för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  