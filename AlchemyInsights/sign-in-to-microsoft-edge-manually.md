---
title: Logga in på Microsoft Edge manuellt
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398675"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Logga in på Microsoft Edge manuellt

Om en användare inte loggas in automatiskt under första körningen kan användaren manuellt logga in via webbläsarens inställningar eller den utfällobaserade identiteten. Använd följande principer för att hantera inloggning:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – För att säkerställa att en användare alltid har en arbetsprofil i Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – Så här begränsar du inloggningen till en uppsättning betrodda konton.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – Inaktivera inloggning eller tvinga användarna att logga in.

