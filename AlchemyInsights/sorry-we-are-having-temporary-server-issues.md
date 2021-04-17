---
title: Åtgärdat Microsoft 365-appar Tyvärr har vi ett meddelande om tillfälliga serverproblem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835289"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="d263a-102">Åtgärda meddelandet "Tyvärr har vi har tillfälliga serverproblem" i Microsoft 365-programmen</span><span class="sxs-lookup"><span data-stu-id="d263a-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="d263a-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="d263a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d263a-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="d263a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d263a-105">Se [URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d263a-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="d263a-106">Gå till **Starta**  >  **kör** och skriv sedan **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="d263a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="d263a-107">Kontrollera att följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="d263a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="d263a-108">Nätverk anslutna enheter – automatisk konfiguration</span><span class="sxs-lookup"><span data-stu-id="d263a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="d263a-109">Nätverkslistetjänst</span><span class="sxs-lookup"><span data-stu-id="d263a-109">Network List Service</span></span>
    - <span data-ttu-id="d263a-110">Information om nätverksplats</span><span class="sxs-lookup"><span data-stu-id="d263a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="d263a-111">Händelselogg i Windows</span><span class="sxs-lookup"><span data-stu-id="d263a-111">Windows Event Log</span></span>

<span data-ttu-id="d263a-112">Om någon av de här tjänsterna inte körs kan du prova att starta den.</span><span class="sxs-lookup"><span data-stu-id="d263a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="d263a-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna kommandotolken med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="d263a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="d263a-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="d263a-114">**sfc /scannow**</span></span>

<span data-ttu-id="d263a-115">Starta om datorn när det här kommandot har avslutats.</span><span class="sxs-lookup"><span data-stu-id="d263a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="d263a-116">Detaljerad information finns i ["Det går tyvärr inte att ansluta till ditt konto. Försök igen senare" när du aktiverar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="d263a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>