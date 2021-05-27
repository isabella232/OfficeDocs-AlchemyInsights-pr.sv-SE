---
title: Felsökning av ediscovery som innehåller fel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676284"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Felsökning av ediscovery som innehåller fel

Har du problem med eDiscovery-eDiscovery-rymmer? Här är några metodtips att tänka på:

- Kontrollera statusen för statusen för håll distribution.  Om statusen **är På (Väntande)** **eller Av (Väntande)** väntar du på att distributionen för väntande är slutförd.
- Koppla eDiscovery och håll uppdateringar i en enda massbegäran i stället för att uppdatera principen flera gånger för varje transaktion.
- Kör Set-CaseHoldPolicy <policyname> -RetryDistribution i Säkerhets- och efterlevnadscenter Powershell. Mer information finns i [Anslut säkerhets- och & PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Anvisningar för hur du kontrollerar de här inställningarna och ytterligare metodtips för att minska och åtgärda eDiscovery-problem som kan innehålla problem finns i [Felsöka fel för eDiscovery-spärrade e-dataidentifiering.](/microsoft-365/compliance/hold-distribution-errors)
Mer information om felsökning av andra vanliga eDiscovery-problem finns i [Undersöka, felsöka och lösa vanliga eDiscovery-problem.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
