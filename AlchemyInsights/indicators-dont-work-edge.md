---
title: Indikatorer fungerar inte med webbläsaren Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887458"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatorer fungerar inte med webbläsaren Edge

När du har skapat en indikator så används den inte av Edge (Smartscreen). Mer information finns i [Skapa indikatorer för IP-adresser och URL:er/domäner.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Steg 1: Kontrollera följande

- Kontrollera att indikatorn är korrekt (inga stavfel i IP/URL, rätt åtgärd och rätt RBAC-grupper).
- Vänta i minst 2 timmar efter att indikatorn har skapats för att ta hänsyn till eventuell fördröjning.
- Bekräfta att systemet/systemerna är onboarded to Microsoft Defender för Endpoint.
- Kontrollera att system kan kommunicera med molnet.
- Kontrollera att Smartscreen är aktiverat och kan nås genom att gå till [testwebbplatsen](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Steg 2: Felsöka det möjliga problemet

- Kontrollera att klienten uppfyller kraven. Mer information finns i [Skapa indikatorer för IP-adresser och URL:er/domäner.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Kontrollera att du kör den senaste versionen av Webbläsaren Edge. Information om hur du tar reda på den senaste [versionen finns i Ta reda på vilken version Microsoft Edge du har](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Starta om Webbläsaren Edge.
- Navigera till den webbplats där en indikator har ställts in. Om webbplatsen inte visas som förväntat fortsätter du till steg 3. 

## <a name="step-3-collect-data"></a>Steg 3: Samla in data

- Samla **in diagnostikdata från MDEClientAnalyzer.** Anvisningar finns i Problem [med onboarding-datorer till Microsoft Defender för Endpoint.](issues-with-onboarding-machines.md)
- Om du är bekväm med att installera och samla in en Fiddler-spårning kan du gå [till Telerik Fiddler](http://www.telerik.com/fiddler).
- Om du föredrar vägledning från Microsoft Support väljer du ikonen Support nedan för att öppna ett supportfall.
