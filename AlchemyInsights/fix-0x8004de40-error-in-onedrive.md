---
title: Åtgärda 0x8004de40 i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649766"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b5114-102">Åtgärda 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="b5114-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b5114-103">Om du kör Windows 7 och får det här felet, uppdatera för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.</span><span class="sxs-lookup"><span data-stu-id="b5114-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="b5114-104">Om du kör Windows 10 och du får ett meddelande om 0x8004de40 med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b5114-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b5114-105">Starta om den dator som påverkas när du är ansluten till din Acitve-katalogdomän.</span><span class="sxs-lookup"><span data-stu-id="b5114-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b5114-106">Om en omstart inte löser problemet kan du ta bort och återansluta till enheten från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5114-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b5114-107">**Obs!** Du bör vara i företagets nätverk när du utför de här stegen.</span><span class="sxs-lookup"><span data-stu-id="b5114-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b5114-108">Utför inte de här stegen när du inte är ansluten till företagets infrastruktur (till exempel när du reser).</span><span class="sxs-lookup"><span data-stu-id="b5114-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="b5114-109">Öppna en upphöjd kommandotolk genom **att välja Start**, högerklicka på **Kommandotolken** och välj **sedan Kör som administratör.**</span><span class="sxs-lookup"><span data-stu-id="b5114-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="b5114-110">Skriv *dsregcmd /leave och* tryck på **Retur.**</span><span class="sxs-lookup"><span data-stu-id="b5114-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="b5114-111">När du är klar skriver *du dsregcmd /join* och trycker på **Retur.**</span><span class="sxs-lookup"><span data-stu-id="b5114-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="b5114-112">Stäng kommandotolken när du är klar.</span><span class="sxs-lookup"><span data-stu-id="b5114-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="b5114-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b5114-113">Reboot the computer, and log into OneDrive.</span></span>