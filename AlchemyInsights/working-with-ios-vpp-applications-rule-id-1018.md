---
title: Arbeta med iOS VPP-program regel-ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688964"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeta med iOS VPP-program

Läs mer om [hur du hanterar iOS-appar som köpts via ett volym köps program med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) för att lära dig mer om funktioner, begränsningar och anvisningar för hur du använder Apples volym köps program och support för det i Microsoft Intune.
  
 **Vanliga problem:** "Jag har tilldelat en iOS-VPP-app till mina användare, men installationen misslyckades."
  
- Det här kan inträffa om en enda VPP-token används i flera providrar för mobila enheter. VPP-token från Apple kan endast användas med en leverantör. Om du har använt en VPP-token med flera leverantörer måste du ladda upp token på nytt.

- Installationen kan även Miss lyckas om det totala antalet installationer överskrider antalet licenser. Om du vill visa en användnings rapport för dina licenser går du till sidan licenser för **Intune-mobilappar** \> **App licenses** . Information om hur du kan återta licenser som används finns i [den här artikeln.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
