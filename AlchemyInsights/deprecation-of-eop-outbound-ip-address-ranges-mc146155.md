---
title: 1065 utfasningen av EOP utgående IP-adress rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404839"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Utfasningen av EOP utgående IP-adressintervall

Vi har upptäckt ett potentiella problem med organisationen som (om de inte åtgärdas genom den 26: e oktober 2018) kan dela e-postflödet i lokala eller externa mål. Som tidigare meddelas för att förenkla hantering av IP-adress område, konsoliderar vi Exchange Online skydd (EOP) IP-adressintervall som används för att skicka och ta emot e-post utanför Office 365. Vår analys visar att en eller flera av de externa e-källor och mål som har angetts i e-flöde kopplingar inte acceptera anslutningar från den IP-adress intervall visas [här](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Handla före oktober 26: e så dessa källor och mål kommer att acceptera anslutningar till och från alla [publicerade EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Mer information om den här förändringen finns i Message Center publicerar [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Anmärkning**: Om du tidigare har använt IP- eller URL-publicering via HTML-, XML och RSS för slutpunkten uppdateringar också migrera till nya webbtjänster för att automatisera dessa typer av uppdateringar. Mer information finns i [Office 365 slutpunkt kategorier och IP-adressen i Office 365 och URL-webbtjänsten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
