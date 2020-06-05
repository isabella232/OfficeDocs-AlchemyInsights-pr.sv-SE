---
title: Åtgärda Microsoft 365-appar Tyvärr har vi ett meddelande om tillfälliga serverproblem
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582721"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="2c31f-102">Åtgärda meddelandet "Tyvärr, vi har tillfälliga serverproblem" visas meddelandet "Tyvärr, vi har tillfälliga serverproblem"</span><span class="sxs-lookup"><span data-stu-id="2c31f-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="2c31f-103">Om du får det här meddelandet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="2c31f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2c31f-104">Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Microsoft 365-appar.</span><span class="sxs-lookup"><span data-stu-id="2c31f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2c31f-105">Se [webbadresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2c31f-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2c31f-106">Gå **Start**till  >  **Startkörning**och skriv sedan **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="2c31f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2c31f-107">Kontrollera att alla följande tjänster körs:</span><span class="sxs-lookup"><span data-stu-id="2c31f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2c31f-108">Automatisk installation av nätverksanslutna enheter</span><span class="sxs-lookup"><span data-stu-id="2c31f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2c31f-109">Tjänsten Nätverkslista</span><span class="sxs-lookup"><span data-stu-id="2c31f-109">Network List Service</span></span>
    - <span data-ttu-id="2c31f-110">Medvetenhet om nätverksplats</span><span class="sxs-lookup"><span data-stu-id="2c31f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2c31f-111">Windows-händelselogg</span><span class="sxs-lookup"><span data-stu-id="2c31f-111">Windows Event Log</span></span>

<span data-ttu-id="2c31f-112">Om en av dessa tjänster inte körs försöker du starta den.</span><span class="sxs-lookup"><span data-stu-id="2c31f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2c31f-113">Om du har problem med att starta tjänsten kör du följande kommando genom att öppna en kommandotolk med förhöjda behörigheter:</span><span class="sxs-lookup"><span data-stu-id="2c31f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2c31f-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="2c31f-114">**sfc /scannow**</span></span>

<span data-ttu-id="2c31f-115">När det här kommandot är klart startar du om datorn.</span><span class="sxs-lookup"><span data-stu-id="2c31f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2c31f-116">Detaljerad information finns i ["Tyvärr, vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="2c31f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>