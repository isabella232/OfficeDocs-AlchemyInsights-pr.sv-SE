---
title: Aktiveringsproblem - Vi kan inte ansluta just nu
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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716190"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="b3345-102">Åtgärda meddelandet "Vi kan inte ansluta just nu"</span><span class="sxs-lookup"><span data-stu-id="b3345-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="b3345-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="b3345-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b3345-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Office-appar.</span><span class="sxs-lookup"><span data-stu-id="b3345-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="b3345-105">Se [Microsofts url:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b3345-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b3345-106">Gå till > **Startkörning**och skriv sedan **services.msc**. **Start**</span><span class="sxs-lookup"><span data-stu-id="b3345-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b3345-107">Kontrollera att alla följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="b3345-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b3345-108">Automatisk installation av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="b3345-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b3345-109">Tjänsten Nätverkslista</span><span class="sxs-lookup"><span data-stu-id="b3345-109">Network List Service</span></span>
    - <span data-ttu-id="b3345-110">Medvetenhet om nätverksplats</span><span class="sxs-lookup"><span data-stu-id="b3345-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b3345-111">Windows-händelselogg</span><span class="sxs-lookup"><span data-stu-id="b3345-111">Windows Event Log</span></span>

<span data-ttu-id="b3345-112">Om en av dessa tjänster inte körs försöker du starta den.</span><span class="sxs-lookup"><span data-stu-id="b3345-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b3345-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="b3345-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b3345-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="b3345-114">**sfc /scannow**</span></span>

<span data-ttu-id="b3345-115">När det här kommandot är klart startar du om datorn.</span><span class="sxs-lookup"><span data-stu-id="b3345-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b3345-116">Detaljerad information finns i ["Tyvärr, vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b3345-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>