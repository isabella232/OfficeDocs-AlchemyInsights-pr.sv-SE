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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581893"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="c6bae-102">Åtgärda meddelandet "Vi kan inte ansluta just nu" i meddelandet "Vi kan inte ansluta just nu"</span><span class="sxs-lookup"><span data-stu-id="c6bae-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="c6bae-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="c6bae-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c6bae-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="c6bae-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="c6bae-105">Se [Microsofts url:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c6bae-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c6bae-106">Gå **Start**till  >  **Startkörning**och skriv sedan **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="c6bae-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c6bae-107">Kontrollera att alla följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="c6bae-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c6bae-108">Automatisk installation av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="c6bae-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c6bae-109">Tjänsten Nätverkslista</span><span class="sxs-lookup"><span data-stu-id="c6bae-109">Network List Service</span></span>
    - <span data-ttu-id="c6bae-110">Medvetenhet om nätverksplats</span><span class="sxs-lookup"><span data-stu-id="c6bae-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c6bae-111">Windows-händelselogg</span><span class="sxs-lookup"><span data-stu-id="c6bae-111">Windows Event Log</span></span>

<span data-ttu-id="c6bae-112">Om en av dessa tjänster inte körs försöker du starta den.</span><span class="sxs-lookup"><span data-stu-id="c6bae-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c6bae-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="c6bae-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c6bae-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="c6bae-114">**sfc /scannow**</span></span>

<span data-ttu-id="c6bae-115">När det här kommandot är klart startar du om datorn.</span><span class="sxs-lookup"><span data-stu-id="c6bae-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c6bae-116">Detaljerad information finns i ["Tyvärr, vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar Office från Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="c6bae-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>