---
title: Regler för minskning av attackytan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676444"
---
# <a name="attack-surface-reduction-rules"></a>Regler för minskning av attackytan

Att utesluta filer eller mappar kan allvarligt minska skyddet som tillhandahålls av minskningsregler för attackytan. Filer som skulle ha blockerats av en regel tillåts köras och ingen rapport eller händelse registreras. Ett undantag gäller för alla regler som tillåter undantag.

ASR-undantag använder samma syntax som Microsoft Defender Antivirus undantag. Mer information finns i [Konfigurera och validera undantag för Microsoft Defender Antivirus genomsökningar](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Om du vill undvika problem [kan du läsa vanliga misstag som du bör undvika när du definierar undantag](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Alla ASR-regler stöder inte undantag. Information om hur du kontrollerar om regeln stöder undantag finns i tabellen [Minskning av attackytan](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regler för minskning av attackytan

Din organisations attackyta omfattar alla platser där en attack kan avslöja organisationsenheter eller nätverk. Att minska attackytan innebär att skydda organisationens enheter och nätverk, vilket lämnar attacker med färre sätt att utföra attacker. Det kan hjälpa att konfigurera regler för att minska attackytan i Microsoft Defender för Endpoint.

Mer information finns i:

- [Mappa ASR-regel-GUID till namn](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Krav för ASR-regler:
    - [Windows 10 Pro, version 1709 eller senare](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, version 1709 eller senare](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, version 1803 (Halvårskanal) eller senare](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifiera rätt undantag som ska tillämpas

1. Leta efter eventID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operational-loggen.

1. Utvärdera blockeringsscenariot och -kontexten och bekräfta att det här scenariot måste avblockas.

1. Läs värdet Path i händelseinformationen, som är det värde som definierar undantaget.
    - Se till att undantaget är så strikt som möjligt.
    - Använd ett jokertecken när det behövs (t.ex. ersätt användarvariabel).

1. Tillämpa undantaget enligt dina behov vid distribution. Mer information finns i [Anpassa regler för att minska attackytan.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Undantag respekteras inte

1. Bestäm om regeln ska stödja undantag. Mer information finns i Regler [för att minska attackytan.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Granska undantag som tillämpas och verifiera med händelsedata för skrivfel eller felupptecknade jokertecken. Mer information finns i [Undantagstyper som stöds](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Om effekten av regeln är för hög kan du flytta tillbaka regeln (tillbaka) till granskningsläge för ytterligare validering. Mer information finns i [Testa hur Microsoft Defender för slutpunktsfunktioner fungerar i granskningsläge.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Samla in supportdata för att öppna ett supportfall med hjälp av det här kommandot:
    
   ** MDEClientAnalyzer.cmd -v**

    Mer information finns i Problem [med onboarding-datorer till Microsoft Defender för slutpunkter.](issues-with-onboarding-machines.md)
