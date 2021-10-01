---
title: Distribuera Microsoft 365-applikationer för delad användning i RDS, Terminal Server eller VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077268"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Distribuera Microsoft 365-applikationer för delad användning i RDS, Terminal Server eller VDI

Om du Microsoft 365-applikationer via Fjärrskrivbordstjänster (RDS), tidigare Terminal Services, måste du:

- Använd enkel korrigering för att aktivera TLS 1.2 som standard om du kör en äldre version av Windows (t.ex. Windows 7 SP1, Windows Server 2008 R2). Mer information om enkel korrigering och mer information finns i Uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)som standard säkra protokoll i WinHTTP i Windows. 
- Ha ett abonnemang som innehåller Microsoft 365-appar för företag (tidigare Office 365 Plus). Till exempel Office 365 E3 eller Microsoft 365 E5, eller ett abonnemang som innehåller skrivbordsversionen av Project eller Visio, till exempel Project Abonnemang 3 eller Visio Abonnemang 2, eller Microsoft 365 Business Premium-abonnemanget, som också innehåller Microsoft 365-applikationer för affärsverksamhet.
- Aktivera aktivering av delad dator. Mer information finns i Översikt [över aktivering av delade datorer för Microsoft 365-applikationer](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Obs!** Om du vill Microsoft 365-applikationer i läget för aktivering på en delad dator laddar du ned [och kör Microsoft-Support- och återställningsassistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal). Mer information om förutsättningar, installationsanvisningar och vägledning för att anpassa installationer med hjälp av distributionsverktyget för Office finns i distribuera Microsoft 365-applikationer med hjälp av [Fjärrskrivbordstjänster.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Information om hur du åtgärdar fel relaterade till aktivering av delad dator finns i:

- [Felsöka problem med aktivering av delad dator Microsoft 365-applikationer](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Återställa Microsoft 365-appar för företagsaktiveringsstatus.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Om du vill installera Microsoft 365-applikationer RDS från Administrationscenter för Microsoft 365, som använder standardinställningarna för installation, gör du så här:

1. Kontrollera vilket Microsoft 365 abonnemang du har. Mer information finns i [Vilken prenumeration har jag?.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. Om det behövs byter du till ett annat Microsoft 365 abonnemang. Mer information finns i [Uppgradera till ett annat abonnemang.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Om Microsoft 365-applikationer har installerats på RDS-servern med andra inkompatibla abonnemang avinstallerar du det genom att gå till **Kontrollpanelen**  >  **Avinstallera ett program.** Om du får problem avinstallerar du genom att hämta [Microsoft Support- och återställningsassistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. På RDS-servern loggar du in på Administrationscenter för Microsoft 365 administratörskonto och [installerar Office](https://portal.office.com/OLS/MySoftware.aspx).

   När Office har installerats ska du inte öppna eller logga in i något Office program.

1. Aktivera aktivering av delad dator på RDS-servern genom att redigera registret:

   1. Högerklicka på Windows i det nedre vänstra hörnet av skärmen och välj **Kör**. Skriv regedit i rutan **Öppna** klicka sedan på **OK**.

   1. När du uppmanas att tillåta Registereditorn att göra ändringar på din enhet väljer du **Ja.**

   1. I Registereditorn, under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, lägger du till strängvärdet **SharedComputerLicensing** med inställningen **1.**

1. Logga in som slutanvändare på RDS-servern och kontrollera att aktivering av delad dator är aktiverad för Microsoft 365-applikationer. 

   Mer information finns i [Kontrollera att aktivering av delade datorer är aktiverat för Microsoft 365-applikationer](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).