---
title: 1065 utfasningen av EOP utgående IP-adress rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492596"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="de93c-102">Utfasningen av EOP utgående IP-adressintervall</span><span class="sxs-lookup"><span data-stu-id="de93c-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="de93c-p101">Vi har upptäckt ett potentiella problem med organisationen som (om de inte åtgärdas genom den 26: e oktober 2018) kan dela e-postflödet i lokala eller externa mål. Som tidigare meddelas för att förenkla hantering av IP-adress område, konsoliderar vi Exchange Online skydd (EOP) IP-adressintervall som används för att skicka och ta emot e-post utanför Office 365. Vår analys visar att en eller flera av de externa e-källor och mål som har angetts i e-flöde kopplingar inte acceptera anslutningar från den IP-adress intervall visas [här](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="de93c-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="de93c-106">Handla före oktober 26: e så dessa källor och mål kommer att acceptera anslutningar till och från alla [publicerade EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="de93c-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="de93c-107">Mer information om den här förändringen finns i Message Center publicerar [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="de93c-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="de93c-p102">**Anmärkning**: Om du tidigare har använt IP- eller URL-publicering via HTML-, XML och RSS för slutpunkten uppdateringar också migrera till nya webbtjänster för att automatisera dessa typer av uppdateringar. Mer information finns i [Office 365 slutpunkt kategorier och IP-adressen i Office 365 och URL-webbtjänsten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="de93c-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

