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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540919"
---
# <a name="how-to-disable-external-groups"></a>Så här inaktiverar du externa grupper

Yammer externa meddelanden gäller Exchange transportregler (ETRs) av förebyggande kontroller för att förhindra företagsinformation från att delas. För att hindra användare från att skapa externa grupper, måste du konfigurera en regel för Exchange transport (ETR) och konfigurera Yammer för att använda Exchange Transport-regel för att blockera externa meddelanden.
  
När du har skapat en regel i Exchange Online administratörscenter, gör så här om du vill ange ETR gäller i Yammer:
  
- Logga in på Yammer som verifierad admin och i **Yammer administratörscenter**, gå till C **innehåll och säkerhet \> säkerhetsinställningar.**

- Markera under **Externa meddelanden** **Tvinga din Exchange Online Exchange transportregler (ETRs) i Yammer.**

- Välj **Save**.

Mer information finns i [Kontrollera externa meddelanden i Yammer-nätverket med Exchange transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  