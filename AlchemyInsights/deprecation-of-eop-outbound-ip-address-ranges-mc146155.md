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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="8cbca-102">Utfasning av EOP-utgående IP-adressintervall</span><span class="sxs-lookup"><span data-stu-id="8cbca-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="8cbca-103">Vi har upptäckt ett potentiellt problem med din organisation som (om den inte korrigeras senast den 26 oktober 2018) kan bryta e-postflödet till dina lokala eller externa destinationer.</span><span class="sxs-lookup"><span data-stu-id="8cbca-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="8cbca-104">Som tidigare kommunicerats, för att förenkla IP-adressintervallhantering, konsoliderar vi IP-adressintervallen (Exchange Online Protection) som används för att skicka och ta emot e-post utanför Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8cbca-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="8cbca-105">Vår analys visar att en eller flera av de externa e-postkällor eller destinationer som du har konfigurerat i e-postflödeskopplingar inte accepterar anslutningar från IP-adressintervallen som visas [här](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="8cbca-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="8cbca-106">Agera före den 26 oktober för att säkerställa att dessa källor och destinationer kommer att acceptera anslutningar till och från alla [publicerade EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="8cbca-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="8cbca-107">Mer information om den här ändringen finns i Inlägg i Message Center som lägger in [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="8cbca-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="8cbca-108">**Om**du tidigare har använt IP- eller URL-publicering via HTML, XML och RSS för slutpunktsuppdateringar bör du också migrera till de nya webbtjänsterna för att automatisera dessa typer av uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="8cbca-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="8cbca-109">Mer information finns i [Microsoft 365-slutpunktskategorier och Microsoft 365 IP-adress- och URL-webbtjänst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="8cbca-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
