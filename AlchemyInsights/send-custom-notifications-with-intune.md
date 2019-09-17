---
title: Skicka anpassade meddelanden med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992330"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Så här skickar du anpassade meddelanden till användare av hanterade iOS-och Android-enheter

Anpassade meddelanden för Intune bearbetas av företagsportalappen på en användares enhet. Appen skapar sedan push-meddelande på den enheten.

Följande är enhets förutsättningar för att stödja mottagandet av anpassade meddelanden och för att appen ska skapa push-meddelandet:

- Enheten måste ha företagsportalappen installerad.  

- Enheten måste tillåta företagsportalappen att skicka push-meddelanden. När appen installeras eller uppdateras uppmanas användaren att tillåta meddelanden.

- Android-enheter måste ha Google Play-tjänster installerade.

- Enheten måste vara registrerad med Intune.

Mer information, inklusive hur du skickar ett meddelande, finns i [funktions dokumentationen](https://docs.microsoft.com/intune/custom-notifications).
