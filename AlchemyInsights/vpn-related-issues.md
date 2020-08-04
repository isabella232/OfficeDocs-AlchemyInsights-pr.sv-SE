---
title: VPN-relaterade problem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555744"
---
# <a name="vpn-related-issues"></a>VPN-relaterade problem

En lyckad implementering av VPN-anslutning för MDM-klienter beror på en distribuerad profil som korrekt återspeglar kraven för VPN-infrastrukturen. För lämpliga inställningar för klientplattformarna som du undersöker finns i: 

[Inställningar för Windows 10 och Windows Holographic device för att lägga till VPN-anslutningar med Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Lägga till VPN-inställningar på iOS- och iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Inställningar för Android-enhet för att konfigurera VPN i Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Lägga till VPN-inställningar på macOS-enheter i Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Om din VPN-profil använder certifikatbaserad autentisering kontrollerar du att rotcertifikat- och klientautentiseringscertifikatprofilerna som är länkade till VPN-profilen har distribuerats.

**Vanliga frågor**

**Jag har distribuerat en VPN-profil till en enhet. Intune visar att det lyckades, men enheten ansluter inte till VPN.**

En lyckad status innebär att Intune har distribuerat profilen som konfigurerad. Dessa konfigurationer kanske inte matchar dina nätverks- och/eller autentiseringskrav. Granska loggar i infrastruktur- och autentiseringstjänsten (på VPN-servern och NPS/Radius-servern) för mer information om anslutningen. Du kan behöva arbeta med nätverksinfrastrukturteamet, eller VPN-leverantören från tredje part, för att samla in och granska loggar.

**När jag konfigurerar en anpassad VPN för iOS görs VPN-funktionen per app inte tillgänglig.**

Vpn per app för iOS-enheter i Intune är för närvarande tillgängligt för en specifik lista över leverantörer och partner, som också måste uppfylla certifikatkraven innan du konfigurerar en VPN per app. Mer information finns i [Konfigurera vpn (Virtual Private Network) per app för iOS/iPadOS-enheter i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Mer information om alla VPN-anslutningstyper i Intune finns i [Skapa VPN-profiler för att ansluta till VPN-servrar i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN utlöses inte när en konfigurerad domän används**

Om du vill testa automatiska VPN-inställningar ställer du in följande värden:

Jag vill göra följande: **Utvärdera varje anslutningsförsök** 

Välj om du vill ansluta: **Anslut om det behövs**

När användare kommer åt dessa domäner: **target** *måldomännamn*

Om ovanstående konfiguration inte lyckas lägger du till följande element:

När den här webbadressen inte kan nås tvingar du till VPN: **BADURL**