---
title: Utfasning av Exchange PowerShell och grundläggande autentisering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015707"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="029ac-102">Utfasning av Exchange PowerShell och grundläggande autentisering</span><span class="sxs-lookup"><span data-stu-id="029ac-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="029ac-103">Om du vill ha den senaste informationen om hur du ansluter till Exchange Online PowerShell utan att använda grundläggande autentisering [går du hit](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="029ac-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="029ac-104">Observera att grundläggande autentisering fortfarande måste aktiveras på klientdatorn.</span><span class="sxs-lookup"><span data-stu-id="029ac-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="029ac-105">Den nya PowerShell V2-modulen använder modern autentisering för att upprätta anslutning och möjliggöra alla REST-baserade V2-cmdletar.</span><span class="sxs-lookup"><span data-stu-id="029ac-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="029ac-106">Utöver V2-cmdletar kan du också komma åt äldre PowerShell-cmdletar (RPS) som kräver en PowerShell-fjärrsession för att upprättas.</span><span class="sxs-lookup"><span data-stu-id="029ac-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="029ac-107">Att upprätta en RPS-session på en Windows-dator kräver grundläggande WinRM-autentisering för att kunna aktiveras på klientdatorn även om modulen använder en mekanism med modern autentisering för att autentisera för tjänsten.</span><span class="sxs-lookup"><span data-stu-id="029ac-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="029ac-108">Pipeline för grundläggande WinRM-autentisering används för att transportera token för modern autentisering.</span><span class="sxs-lookup"><span data-stu-id="029ac-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="029ac-109">Om grundläggande WinRM-autentisering är inaktiverat på klientdatorn fortsätter de nya V2-cmdletar att fungera (men inte de äldre RPS-cmdletarna).</span><span class="sxs-lookup"><span data-stu-id="029ac-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
