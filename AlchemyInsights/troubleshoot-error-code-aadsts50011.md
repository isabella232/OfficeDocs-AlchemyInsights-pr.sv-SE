---
title: Felsöka felkod AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038060"
---
# <a name="troubleshoot-error-code-aadsts50011"></a>Felsöka felkod AADSTS50011

Lös AADSTS50011-felet genom att utföra det rekommenderade steget som beskrivs nedan.

**AADSTS50011**: InvalidReplyTo – Svarsadressen saknas, är felaktigt konfigurerad eller matchar inte svarsadresser som konfigurerats för appen.

Som en lösning ser du till att lägga till den här svarsadressen som saknas i Azure Active Directory-appen (AD) eller har någon som har behörighet att hantera programmet i AD gör detta åt dig. Mer information finns i felsökningsartikeln för felet [AADSTS50011.](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch)