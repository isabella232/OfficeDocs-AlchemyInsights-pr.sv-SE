---
title: Felsöka Microsoft Defender för Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801464"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a>Felsöka Microsoft Defender för Office 365

- Märker du fördröjningar i leverans av meddelanden? Använd alternativet [dynamisk leverans](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i policyn för säker användning för ATP. Detta hjälper till att undvika meddelande fördröjningar när du skyddar mottagare från skadliga filer.

- Vill du rapportera falsk positiv eller falsk negativ till Microsoft? Använd den här [länken](https://www.microsoft.com/wdsi/filesubmission/) om du vill skicka filer för analys.

- Visste du att du kan aktivera skydd mot säkra Länkar för intern e-post som skickas mellan mottagarna inom din organisation? Gör så här:

  1. Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhets administratörs konto.

  2. Välj **policy** Safe Links i det vänstra navigerings fönstret under **Threat Management** \> **Safe Links** .

  3. I de **principer som gäller för hela avsnittet organisation** väljer du policy och klickar på **Redigera** .

  4. Under **Inställningar** aktiverar **du Använd Safe Links för meddelanden som skickas inom organisationen** .
