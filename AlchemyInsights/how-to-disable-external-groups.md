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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384843"
---
# <a name="how-to-disable-external-groups"></a>Så här inaktiverar du externa grupper

Yammer externa meddelanden gäller Exchange transportregler (ETRs) av förebyggande kontroller för att förhindra företagsinformation från att delas. För att hindra användare från att skapa externa grupper, måste du konfigurera en regel för Exchange transport (ETR) och konfigurera Yammer för att använda Exchange Transport-regel för att blockera externa meddelanden.
  
När du har skapat en regel i Exchange Online administratörscenter, gör så här om du vill ange ETR gäller i Yammer:
  
- Logga in på Yammer som verifierad admin och i **Yammer administratörscenter**, gå till C **innehåll och säkerhet \> säkerhetsinställningar.**

- Markera under **Externa meddelanden** **Tvinga din Exchange Online Exchange transportregler (ETRs) i Yammer.**

- Välj **Save**.

Mer information finns i [Kontrollera externa meddelanden i Yammer-nätverket med Exchange transportregler](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  