---
title: 1065 utfasning av EOP utgående IP-adress rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806813"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Utfasning av utgående IP-adressintervall för EOP

Vi har upptäckt ett möjligt problem med din organisation (om den inte rättats till i oktober 26th, 2018) kan du dela upp e-postflödet till dina lokala eller externa destinationer. Som tidigare kommunicerats, för att förenkla hanteringen av IP-adressintervallet, konsoliderar vi de IP-adressintervall för Exchange Online Protection (EOP) som används för att skicka och ta emot e-post utanför Microsoft 365. I vår analys anges att en eller flera externa e-postkällor eller destinationer som du har konfigurerat i e-postflöden inte accepterar anslutningar från IP-adressintervall som visas [här](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Agera före oktober 26th för att säkerställa att dessa källor och destinationer accepterar anslutningar till och från alla [publicerade EOP-IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Om du vill ha mer information om den här ändringen kan du läsa i meddelande Center publicerar [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Obs!** om du tidigare använde IP-eller URL-publicering via HTML-, XML-och RSS för slut punkts uppdateringar bör du även migrera till de nya webb tjänsterna för att automatisera dessa typer av uppdateringar. Mer information finns i [Microsoft 365-slutpunktsservrar och microsoft 365 IP Address and URL Web Service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
