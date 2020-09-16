---
title: Aktiverings problem – vi kan inte ansluta just nu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726001"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="bf0cf-102">Åtgärdar Microsoft 365-apparna "det går inte att ansluta just nu"</span><span class="sxs-lookup"><span data-stu-id="bf0cf-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="bf0cf-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="bf0cf-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="bf0cf-104">Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Internet åtkomst till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="bf0cf-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="bf0cf-105">Se [URL-adresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="bf0cf-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="bf0cf-106">Gå till **Start**  >  **Kör**och skriv **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="bf0cf-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="bf0cf-107">Kontrol lera att följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="bf0cf-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="bf0cf-108">Automatisk konfiguration av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="bf0cf-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="bf0cf-109">Tjänsten nätverks lista</span><span class="sxs-lookup"><span data-stu-id="bf0cf-109">Network List Service</span></span>
    - <span data-ttu-id="bf0cf-110">Nätverks plats medvetenhet</span><span class="sxs-lookup"><span data-stu-id="bf0cf-110">Network Location Awareness</span></span>
    - <span data-ttu-id="bf0cf-111">Windows-händelseloggen</span><span class="sxs-lookup"><span data-stu-id="bf0cf-111">Windows Event Log</span></span>

<span data-ttu-id="bf0cf-112">Om någon av de här tjänsterna inte körs kan du försöka starta den.</span><span class="sxs-lookup"><span data-stu-id="bf0cf-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="bf0cf-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommando tolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="bf0cf-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="bf0cf-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="bf0cf-114">**sfc /scannow**</span></span>

<span data-ttu-id="bf0cf-115">Starta om datorn när det här kommandot är klart.</span><span class="sxs-lookup"><span data-stu-id="bf0cf-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="bf0cf-116">Detaljerad information finns i ["det går inte att ansluta till ditt konto. Försök igen senare "visas när du aktiverar Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="bf0cf-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>