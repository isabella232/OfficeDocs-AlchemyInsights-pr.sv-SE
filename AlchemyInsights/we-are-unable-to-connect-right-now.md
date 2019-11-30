---
title: Aktiveringsproblem-vi kan inte ansluta just nu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628260"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="28776-102">Fastställande av Office Apps "vi kan inte ansluta just nu" meddelande</span><span class="sxs-lookup"><span data-stu-id="28776-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="28776-103">Om det här meddelandet visas provar du följande:</span><span class="sxs-lookup"><span data-stu-id="28776-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="28776-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internet-åtkomst till Office-appar.</span><span class="sxs-lookup"><span data-stu-id="28776-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="28776-105">Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="28776-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="28776-106">Gå till **Start** > **Run**och skriv **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="28776-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="28776-107">Kontrollera att följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="28776-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="28776-108">Automatisk konfigurering av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="28776-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="28776-109">Network List Service</span><span class="sxs-lookup"><span data-stu-id="28776-109">Network List Service</span></span>
    - <span data-ttu-id="28776-110">Nätverksplats medvetenhet</span><span class="sxs-lookup"><span data-stu-id="28776-110">Network Location Awareness</span></span>
    - <span data-ttu-id="28776-111">Händelseloggen för Windows</span><span class="sxs-lookup"><span data-stu-id="28776-111">Windows Event Log</span></span>

<span data-ttu-id="28776-112">Om någon av dessa tjänster inte körs försöker du starta den.</span><span class="sxs-lookup"><span data-stu-id="28776-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="28776-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="28776-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="28776-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="28776-114">**sfc /scannow**</span></span>

<span data-ttu-id="28776-115">När det här kommandot har slutförts startar du om datorn.</span><span class="sxs-lookup"><span data-stu-id="28776-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="28776-116">Mer information finns i ["Tyvärr kan vi inte ansluta till ditt konto. Försök igen senare "felmeddelande när du aktiverar Office från Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="28776-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>