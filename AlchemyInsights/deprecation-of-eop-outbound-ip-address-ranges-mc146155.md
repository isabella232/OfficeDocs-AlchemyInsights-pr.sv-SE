---
title: 1065 utfasning av EOP utgående IP-adressintervallMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031280"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Utfasning av utgående IP-adressintervall för EOP

Vi har upptäckt ett potentiellt problem med din organisation som (om inte korrigerats av den 26 oktober 2018) kan bryta e-postflödet till dina lokala eller externa destinationer. Som tidigare kommunicerat konsoliderar vi IP-adressintervallen för Exchange Online Protection (EOP) som används för att skicka och ta emot e-post utanför Microsoft 365. Analysen visar att en eller flera av de externa e-postkällor eller -mål som du har konfigurerat i e-postflödesanslutningar inte accepterar anslutningar från de IP-adressintervall som visas [här.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Agera före 26 oktober för att säkerställa att dessa källor och destinationer accepterar anslutningar till och från alla [publicerade EOP IP-adresser.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Mer information om den här ändringen finns i Inlägg i Meddelandecenter [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Obs!** Om du tidigare har använt IP- eller URL-publicering via HTML, XML och RSS för slutpunktsuppdateringar bör du även migrera till de nya webbtjänsterna för att automatisera dessa typer av uppdateringar. Mer information finns i Microsoft 365 [kategorier och url-Microsoft 365 IP-adress och URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
