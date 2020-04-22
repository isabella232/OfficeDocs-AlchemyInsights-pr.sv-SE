---
title: 1065 Utfasning av EOP utgående IP-adressintervallMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704615"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Utfasning av EOP-utgående IP-adressintervall

Vi har upptäckt ett potentiellt problem med din organisation som (om den inte korrigeras senast den 26 oktober 2018) kan bryta e-postflödet till dina lokala eller externa destinationer. Som tidigare kommunicerats, för att förenkla IP-adressintervallhantering, konsoliderar vi IP-adressintervallen (Exchange Online Protection) som används för att skicka och ta emot e-post utanför Microsoft 365. Vår analys visar att en eller flera av de externa e-postkällor eller destinationer som du har konfigurerat i e-postflödeskopplingar inte accepterar anslutningar från IP-adressintervallen som visas [här](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Agera före den 26 oktober för att säkerställa att dessa källor och destinationer kommer att acceptera anslutningar till och från alla [publicerade EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Mer information om den här ändringen finns i Inlägg i Message Center som lägger in [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Om**du tidigare har använt IP- eller URL-publicering via HTML, XML och RSS för slutpunktsuppdateringar bör du också migrera till de nya webbtjänsterna för att automatisera dessa typer av uppdateringar. Mer information finns i [Microsoft 365-slutpunktskategorier och Microsoft 365 IP-adress- och URL-webbtjänst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
