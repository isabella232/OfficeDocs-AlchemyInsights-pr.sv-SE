---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971033"
---
# <a name="verify-your-domain"></a>Verify your domain

 **Posten har förmodligen inte uppdaterats på Internet.**
  
Vanligtvis kan vi se den nya posten efter bara några minuter, men ibland kan det ta upp till några timmar. 
  
- Om du redan har väntat så länge kontrollerar du att du har kopierat och klistrat in det exakta värdet i TXT-verifieringsposten hos din DNS-värd. Ett vanligt problem är att man inte har tagit med "MS ="-delen av posten. Vi behöver den också!

- På vissa DNS-värdar måste du vidta extra åtgärd för att spara zonfilen (där DNS-posten lagras) så att den uppdateras på Internet. Kontrollera att du har sparat ändringarna så att Microsoft kan se och verifiera posten.
