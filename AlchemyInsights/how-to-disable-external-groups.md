---
title: Inaktivera externa grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720786"
---
# <a name="how-to-disable-external-groups"></a>Inaktivera externa grupper

Yammer externa meddelanden tillämpar Exchange Transport Rules (ETRs), en uppsättning proaktiva kontroller för att förhindra att företagsinformation delas. För att begränsa användare från att skapa externa grupper måste du konfigurera en Exchange-transportregel (ETR) och sedan konfigurera Yammer så att den använder Exchange Transport-regeln för att blockera externa meddelanden.
  
När du har skapat en regel i Administrationscentret för Exchange Online följer du dessa steg för att ange att ETR ska gälla i Yammer:
  
- Logga in på Yammer som verifierad administratör och gå till **säkerhetsinställningarna \> för C-innehåll och säkerhet** i **Administrationscentret för Yammer.**

- Under **Externa meddelanden**väljer du **Framtvinga dina ETR-regler för Exchange Online Exchange Transport (i Yammer.**

- Välj **Save**.

Mer information finns [i Inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  