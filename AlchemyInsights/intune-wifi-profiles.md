---
title: Intune Wi-Fi-profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555815"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi-profiler

En lyckad implementering av Wi-Fi-anslutning för MDM-klienter beror på en korrekt distribuerad profil som återspeglar kraven för företagets Wi-Fi-infrastruktur. Information om hur du granskar lämpliga inställningar för klientplattformarna som du undersöker finns i: 

[Lägga till Wi-Fi-inställningar för enheter som kör Android i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Lägga till Wi-Fi-inställningar för Android Enterprise-dedikerade och fullständigt hanterade enheter i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Lägga till Wi-Fi-inställningar för iOS- och iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Lägga till Wi-Fi-inställningar för Windows 10 och senare enheter i Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importera Wi-Fi-inställningar för Windows-enheter i Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Vanliga frågor**

**Jag distribuerar en Wi-Fi-profil som är beroende av ett distribuerat certifikat som anges i Wi-Fi-profilen. Konfigurationsprofilerna visar dock en felstatus.**

Kontrollera att enheten har tagit emot certifikatet.

1. Gå till **Alla enheter** i Intune och välj **enhetskonfigurationen**> enhet .

2. Kontrollera att alla förväntade profiler visas och i ett framgångsrikt tillstånd.

3. Om du har mellanliggande certifikat i certifikatkedjan för en Android-profil kontrollerar du att de distribueras till Android-enheter.

    Om du vill kontrollera certifikatstatusen går du till **Enhetskonfigurationsprofiler**  >  **Profiles**  >  **android mellanliggande certifikatutfärdaregenskaper**  >  **Properties**  >  **Trusted Certificate**.

Om du fortsätter att se fel läser du procedurerna och felsökningsavsnitten. Mer information finns i [Översikt för felsökning av SCEP-certifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Jag har distribuerat en Wi-Fi-profil till en enhet. Intune visar att det lyckades, men enheten ansluter inte till Wi-Fi.**

En lyckad status innebär att Intune har distribuerat profilen som konfigurerad. Dessa konfigurationer kanske inte matchar dina nätverks- och/eller autentiseringskrav. Mer information om anslutningens försök finns i infrastruktur- och autentiseringstjänsten (på Wi-Fi-åtkomstpunktsstyrenheten och NPS/Radius-servern). Du kanske måste arbeta med nätverksinfrastrukturteamet, eller wi-fi-leverantören från tredje part, för att samla in och granska loggar.