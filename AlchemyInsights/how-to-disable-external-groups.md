---
title: Inaktivera externa grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015638"
---
# <a name="how-to-disable-external-groups"></a>Inaktivera externa grupper

Yammer för externa meddelanden Exchange i Transportregler (ETR-regler), en uppsättning förebyggande kontroller för att förhindra att företagsinformation delas. Om du vill hindra användare från att skapa externa grupper måste du konfigurera en Exchange-transportregel (ETR) och sedan konfigurera Yammer så att den använder Exchange-transportregeln för att blockera externa meddelanden.
  
När du har skapat en regel i Exchange Online-administrationscentret följer du de här anvisningarna för att ange att ETR ska användas i Yammer:
  
- Logga in på Yammer som verifierad administratör. I administrationscentret för **Yammer** går du till C-Inställningar. **\>**

- Under **Externa meddelanden** väljer du Tillämpa **Exchange Online Exchange-transportregler (ETR-regler) i Yammer.**

- Välj **Spara**.

Mer information finns i Inaktivera [externa meddelanden i ett Yammer nätverk.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  