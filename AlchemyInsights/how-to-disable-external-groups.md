---
title: Så här inaktiverar du externa grupper
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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704146"
---
# <a name="how-to-disable-external-groups"></a>Så här inaktiverar du externa grupper

I externa meddelanden i Yammer används Exchange Transport Rules (ETR), en uppsättning proaktiva kontroller för att förhindra att företags informationen delas. För att hindra användare från att skapa externa grupper måste du konfigurera en Exchange-Exchange och sedan konfigurera Yammer så att externa meddelanden blockeras.
  
När du har skapat en regel i administrations centret för Exchange Online följer du de här stegen för att ange att Exchange ska tillämpas i Yammer:
  
- Logga in på Yammer som verifierad administratör och gå till **säkerhet och säkerhets \> Inställningar** i **administrations centret för Yammer**.

- Under **externa meddelanden**väljer **du tvinga fram Exchange-ETR för Exchange Online i Yammer.**

- Välj **Save**.

Mer information finns i [inaktivera externa meddelanden i ett Yammer-nätverk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  