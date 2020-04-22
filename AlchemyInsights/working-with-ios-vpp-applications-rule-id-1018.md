---
title: Arbeta med iOS VPP Applications Rule ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719975"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeta med iOS VPP-program

Läs [så här hanterar du iOS-appar som köpts via ett volymköpsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) om du vill veta mer om funktioner, begränsningar och steg för att använda Apple Volume Purchase Program och stödet för det i Microsoft Intune.
  
 **Vanliga frågor:** "Jag tilldelade en iOS VPP-app till mina användare, men installationen misslyckades."
  
- Detta kan inträffa om en enda VPP-token används över flera leverantörer av hantering av mobila enheter. VPP-tokens från Apple får endast användas hos en leverantör. Om du använde en VPP-token med flera providers måste du ladda upp token till Intune igen.

- Installationen kan också misslyckas om det totala antalet installationer överstiger antalet licenser. Om du vill visa en användningsrapport för dina licenser går du till sidan Licenser för **Intune Mobile** \> **apps-appar.** Mer information om hur du återkräver licenser som används finns i [den här artikeln.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
