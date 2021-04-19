---
title: Lösa SMTP-autentiseringsproblem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826433"
---
# <a name="solving-smtp-authentication-issues"></a>Lösa SMTP-autentiseringsproblem

Om du får felen 5.7.57 eller 5.7.3 när du försöker skicka SMTP-e-post och autentisera med en klient eller ett program finns det några saker du bör kontrollera:

- Autentiserad sändning via SMTP kan vara inaktiverad i klientorganisationen eller i postlådan som du försöker använda (kontrollera båda inställningarna). Mer information finns i Aktivera [eller inaktivera autentiserad SÄNDNING VIA SMTP-klient.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Kontrollera om [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) är aktiverat för din klientorganisation. om den är aktiverad kommer SMTP-autentisering med hjälp av grundläggande autentisering (kallas även äldre, detta kommer att använda användarnamn och lösenord) att misslyckas.
