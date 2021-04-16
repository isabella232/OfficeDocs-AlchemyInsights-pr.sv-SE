---
title: Utfasning av Exchange PowerShell och grundläggande autentisering
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813490"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="8b812-102">Utfasning av Exchange PowerShell och grundläggande autentisering</span><span class="sxs-lookup"><span data-stu-id="8b812-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="8b812-103">Om du vill ha den senaste informationen om hur du ansluter till Exchange Online PowerShell utan att använda grundläggande autentisering [går du hit](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="8b812-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="8b812-104">PowerShell V2-modulen använder inte grundläggande autentisering.</span><span class="sxs-lookup"><span data-stu-id="8b812-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="8b812-105">Observera att grundläggande autentisering fortfarande måste aktiveras på klientdatorn.</span><span class="sxs-lookup"><span data-stu-id="8b812-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="8b812-106">Den nya PowerShell V2-modulen använder modern autentisering för att upprätta anslutning och möjliggöra alla REST-baserade V2-cmdletar.</span><span class="sxs-lookup"><span data-stu-id="8b812-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="8b812-107">Utöver V2-cmdletar kan du också komma åt äldre PowerShell-cmdletar (RPS) som kräver en PowerShell-fjärrsession för att upprättas.</span><span class="sxs-lookup"><span data-stu-id="8b812-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="8b812-108">Att upprätta en RPS-session på en Windows-dator kräver grundläggande WinRM-autentisering för att kunna aktiveras på klientdatorn även om modulen använder en mekanism med modern autentisering för att autentisera för tjänsten.</span><span class="sxs-lookup"><span data-stu-id="8b812-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="8b812-109">Pipeline för grundläggande WinRM-autentisering används för att transportera token för modern autentisering.</span><span class="sxs-lookup"><span data-stu-id="8b812-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="8b812-110">Om grundläggande WinRM-autentisering är inaktiverat på klientdatorn fortsätter de nya V2-cmdletar att fungera (men inte de äldre RPS-cmdletarna).</span><span class="sxs-lookup"><span data-stu-id="8b812-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
