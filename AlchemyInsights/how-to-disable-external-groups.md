---
title: Så här inaktiverar du externa grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739511"
---
# <a name="how-to-disable-external-groups"></a>Så här inaktiverar du externa grupper

Yammer externa meddelanden gäller Exchange Transport regler (ETRs), en uppsättning proaktiva kontroller för att förhindra att företagsinformation delas. För att begränsa användare från att skapa externa grupper, måste du konfigurera en Exchange Transport-regel (ETR) och sedan konfigurera Yammer att använda Exchange Transport-regel för att blockera externa meddelanden.
  
När du har skapat en regel i Exchange Online Admin Center, Följ dessa steg för att ange ETR ska tillämpas i Yammer:
  
- Logga in på Yammer som en verifierad administratör och i **Administrationscenter för Yammer**, gå till C **innehåll och \> säkerhet säkerhetsinställningar.**

- Under **externa meddelanden**, Välj **Framtvinga Exchange Online Exchange Transport-regler (ETRS) i Yammer.**

- Välj **Save**.

Mer information finns [i inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  