---
title: Installera Office på en terminalserver-olicensierad
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663135"
---
# <a name="installing-office-on-a-terminal-server"></a>Installera Office på en terminalserver

För distribution av Microsoft 365-appar för företag på en Windows Server med fjärr skrivbords tjänster (RDS), tidigare kallat Terminal Services:
  
- Du måste ha en Microsoft 365-prenumeration som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5. Microsoft 365-apparna för företag och Microsoft 365-appar för företag Premium-program inkluderar inte Microsoft 365-appar för företag.

- Du måste aktivera [delad dator aktivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Om du vill installera Microsoft 365-appar för företag på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, gör du följande:

> [!TIP]
> Du kan också ladda ned och köra [Microsoft-assistenten för support och återställning](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365-appar för företag i aktiverings läget för delad dator.
  
1. Kolla vilken Microsoft 365-prenumeration du har. [Lär dig hur](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Om det behövs byter du till en annan Microsoft 365-prenumeration. [Lär dig hur](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Om Office redan är installerat på RDS-servern med andra Microsoft 365-abonnemang avinstallerar du det. Till exempel genom att gå till kontroll panelen \> Avinstallera ett program. Avinstallera med [Microsoft support-och återställnings assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du stöter på problem.

4. Logga in på administrations centret för Microsoft 365 med ditt administratörs konto och [Installera Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).

5. När Office är installerat kan du ***inte öppna eller logga*** in på något Office-program.

6. Aktivera delad dator aktivering på RDS-servern genom att redigera registret genom att följa de här stegen:

1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj Kör. I rutan Öppna skriver du **regedit**och väljer sedan OK.

2. Välj Ja när du uppmanas att tillåta att Registereditorn gör ändringar på enheten.

3. I Registereditorn lägger du till ett sträng värde för **SharedComputerLicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. ***Logga in som slutanvändare*** på RDS-servern och [kontrol lera att aktivera delad dator är aktiverat för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Mer information om förutsättningar, installations anvisningar och vägledning om anpassade installationer med hjälp av distributions verktyget för Office finns i [distribuera Microsoft 365-appar för företag med hjälp av fjärr skrivbords tjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Information om hur du åtgärdar problem med att aktivera en delad dator finns i [Felsöka problem med delad dator aktivering för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  