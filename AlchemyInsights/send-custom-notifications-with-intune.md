---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720664"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Skicka anpassade meddelanden till användare av hanterade iOS-och Android-enheter

Anpassade meddelanden för Intune bearbetas av företagsportalsappen på en användares enhet. Programmet skapar sedan push-meddelandet på den enheten.

Följande är enhets förutsättningar för att stödja mottagning av anpassade meddelanden, och för appen att skapa push-meddelandet:

- Programmet måste ha företagsportalsappen installerat.  

- Enheten måste tillåta att företagsportalsappen skickar push-meddelanden till företags portalen. När appen installeras eller uppdateras uppmanas användaren att tillåta aviseringar.

- Google Play Services måste vara installerat på Android-enheter.

- Enheten måste vara registrerad med Intune.

Mer information om hur du skickar ett meddelande finns i dokumentationen för [funktionerna](https://docs.microsoft.com/intune/custom-notifications).
