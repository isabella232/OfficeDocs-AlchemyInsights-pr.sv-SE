---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886875"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Så här skickar du anpassade meddelanden till användare av hanterade iOS-och Android-enheter

Anpassade meddelanden för Intune bearbetas av företagsportalappen på en användares enhet. Appen skapar sedan push-meddelande på den enheten.

Följande är enhets förutsättningar för att stödja mottagandet av anpassade meddelanden och för att appen ska skapa push-meddelandet:

- Enheten måste ha företagsportalappen installerad.  

- Enheten måste tillåta företagsportalappen att skicka push-meddelanden. När appen installeras eller uppdateras uppmanas användaren att tillåta meddelanden.

- Android-enheter måste ha Google Play-tjänster installerade.

- Enheten måste vara registrerad med Intune.

Mer information, inklusive hur du skickar ett meddelande, finns i [funktions dokumentationen](https://docs.microsoft.com/intune/custom-notifications).
