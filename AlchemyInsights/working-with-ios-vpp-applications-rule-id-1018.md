---
title: Arbeta med iOS VPP program regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558023"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeta med iOS VPP program

Läsa om [hur du hanterar iOS-appar som köpts via en inköpsvolym program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) du lär dig mer om funktioner, villkor och åtgärder för att kontrollera användning av Apple volym köpa Program och stöd för den i Microsoft Intune.
  
 **Vanliga problem:** ”Jag har tilldelat en VPP iOS-app för användarna, men installationen misslyckades”.
  
- Detta kan inträffa om en enda VPP-token används över flera leverantörer för hantering av mobil enhet. VPP-token från Apple kan endast användas med en provider. Om du använde en VPP-token med flera leverantörer måste du överföra token till Intune.

- Installationen misslyckas även om det totala antalet installationer av överskrider antalet licenser. Om du vill visa en användningsrapport för din licens, gå till **Intune Mobile apps** \> **App licenser** sida. Information om hur du frigör licenser används, se [i den här artikeln.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
