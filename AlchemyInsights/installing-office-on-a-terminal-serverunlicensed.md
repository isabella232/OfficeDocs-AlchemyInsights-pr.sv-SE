---
title: Installera office på en Terminal Server - olicensierade
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492371"
---
# <a name="installing-office-on-a-terminal-server"></a>Installera Office på en Terminal-Server

För distribution av Office 365 ProPlus på en Windows-Server med hjälp av Remote Desktop Services (RDS), tidigare kallad Terminal Services:
  
- Du måste ha en Office 365-plan som innehåller Office 365 ProPlus, till exempel Office 365 Enterprise E3 eller Enterprise E5. Ta inte med Office 365 ProPlus Office 365 Business och Office 365 Business Premium planer.
    
- Du måste aktivera [delad dator](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Om du vill installera Office 365 ProPlus på klientåtkomstlicenser från Office 365-portalen ** *som använder standardinställningarna för installationen* **, gör du så här: 
  
1. Kontrollera vilken Office 365-plan du har. [Lär dig mer om hur](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Om det behövs, växla till en annan Office 365-plan. [Lär dig mer om hur](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Om Office har installerats på RDS-server med hjälp av andra Office 365-planer, avinstallera den. Till exempel Gå till Kontrollpanelen genom att \> avinstallera ett program. Avinstallera med hjälp av [Microsoft Support och återställning assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du kör till problem. 
    
4. Logga in på Office 365-portalen med ditt administratörskonto och [installera Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)på RDS-server.
    
5. När Office har installerats ** *inte öppna eller logga in* ** för alla Office-program. 
    
6. Aktivera delade aktivering på RDS-server genom att redigera registret så här:
    
1. Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj kör. Skriv **regedit**i rutan Öppna och klicka sedan på OK. 
    
2. Välj Ja när du uppmanas att tillåta Registereditorn att göra ändringar i din enhet.
    
3. I Registereditorn kan du lägga till ett strängvärde av **SharedComputerLicensing** med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. På RDS-server ** *Logga in som en användare* ** och [Kontrollera att delade aktivering är aktiverat för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Mer information om förutsättningar, instruktioner och riktlinjer för anpassade installationer med hjälp av verktyget Office Deployment finns i [Distribuera Office 365 ProPlus med hjälp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Åtgärda fel som är relaterade till delade aktivering finns i [Felsöka problem med delade aktivering för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

