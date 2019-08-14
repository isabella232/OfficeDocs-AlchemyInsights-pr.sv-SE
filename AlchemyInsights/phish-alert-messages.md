---
title: 2491 alert e-postmeddelanden från Phish levereras innehavare eller användare åsidosätter principen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391564"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alert e-postmeddelanden från Phish levereras innehavare eller användare åsidosätter principen

En varning standardprincipen ”Phish levererad på Åsidosätt innehavare eller användare” har ångrats till hyresgäster med licenser för Office 365 ATP P1 och P2. Här är stegen för att undersöka om du fått denna varning:

1. Meddelande, klicka på **Visa varning** att gå till sidan **meddelanden** i säkerhet & regelefterlevnadscentret.

2. Markera aviseringen till finns alternativ för att **Visa meddelandelista** eller **Visa meddelanden i Explorer**. Båda dessa alternativ om du vill ha information om meddelandet, som innehåller meddelande-ID. Observera att länken hot Explorer automatiskt ska filtrera meddelanden som matchar aviseringsvillkoren. Du kan behöva justera Datumfilter i Explorer hot.

Phishing-meddelandet levererades på grund av en manuellt konfigurerad åsidosättning:

- En tillåtna avsändare eller domän som anges av användaren.

- En tillåtna avsändare eller domän som anges av admin i en policy mot skräppost.

- En tillåtna IP-adress i en princip för filtret.

- E-post flöde regel (kallas även en transportregel) som är konfigurerad för att tillåta meddelanden i.

Om du tror att meddelandet var felaktigt markerad som nätfiske, använda Outlook [tillägget rapportmeddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att överlämna prover av meddelande till Microsoft.
