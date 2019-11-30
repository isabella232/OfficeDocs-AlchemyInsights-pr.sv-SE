---
title: Åtgärda Office-appar tyvärr, vi har tillfälliga Server problem meddelande
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628008"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="ec544-102">Fastställande av Office Apps "Tyvärr, vi har tillfälliga Server problem" meddelande</span><span class="sxs-lookup"><span data-stu-id="ec544-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="ec544-103">Om det här meddelandet visas provar du följande:</span><span class="sxs-lookup"><span data-stu-id="ec544-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ec544-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internet-åtkomst till Office-appar.</span><span class="sxs-lookup"><span data-stu-id="ec544-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ec544-105">Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ec544-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ec544-106">Gå till **Start** > **Run**och skriv **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="ec544-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ec544-107">Kontrollera att följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="ec544-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ec544-108">Automatisk konfigurering av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="ec544-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ec544-109">Network List Service</span><span class="sxs-lookup"><span data-stu-id="ec544-109">Network List Service</span></span>
    - <span data-ttu-id="ec544-110">Nätverksplats medvetenhet</span><span class="sxs-lookup"><span data-stu-id="ec544-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ec544-111">Händelseloggen för Windows</span><span class="sxs-lookup"><span data-stu-id="ec544-111">Windows Event Log</span></span>

<span data-ttu-id="ec544-112">Om någon av dessa tjänster inte körs försöker du starta den.</span><span class="sxs-lookup"><span data-stu-id="ec544-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ec544-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="ec544-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ec544-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="ec544-114">**sfc /scannow**</span></span>

<span data-ttu-id="ec544-115">När det här kommandot har slutförts startar du om datorn.</span><span class="sxs-lookup"><span data-stu-id="ec544-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ec544-116">Mer information finns i ["Tyvärr kan vi inte ansluta till ditt konto. Försök igen senare "felmeddelande när du aktiverar Office från Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ec544-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>