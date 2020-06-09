---
title: 'Fel: Reglerna på den här datorn matchar inte'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618031"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="5fd17-102">Fel: Reglerna på den här datorn matchar inte</span><span class="sxs-lookup"><span data-stu-id="5fd17-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="5fd17-103">Information om hur du ser uppdaterad status för det här kända problemet finns [i Reglerna på den här datorn matchar inte reglerna för Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="5fd17-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="5fd17-104">Outlook-teamet har implementerat en korrigering i Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="5fd17-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="5fd17-105">Korrigeringen är redan på Insider Fast och kommer att gå till Monthly Channel i slutet av juni 2020.</span><span class="sxs-lookup"><span data-stu-id="5fd17-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="5fd17-106">När du har den fasta bygga kan du få prompten "Vilka regler vill du behålla" en sista gång.</span><span class="sxs-lookup"><span data-stu-id="5fd17-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="5fd17-107">Välj Server när du uppmanas att göra det och gå sedan tillbaka till Outlook och aktivera alla regler som har inaktiverats igen.</span><span class="sxs-lookup"><span data-stu-id="5fd17-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="5fd17-108">Tills korrigeringen är tillgänglig kan du använda följande lösning:</span><span class="sxs-lookup"><span data-stu-id="5fd17-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="5fd17-109">**Lösning**: I de senaste rapporterna har problemet uppstått för dem som bara har skapat klientregler i Outlook-skrivbordet.</span><span class="sxs-lookup"><span data-stu-id="5fd17-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="5fd17-110">Om du fortsätter att stöta på problemet kan du överväga att ta bort reglerna och sedan skapa och redigera regler endast i OWA (Outlook Web App) tills problemet är löst.</span><span class="sxs-lookup"><span data-stu-id="5fd17-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="5fd17-111">Om du inte kan ta bort reglerna manuellt kan du köra ett Outlook-kommando när du startar Outlook genom att köra Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="5fd17-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="5fd17-112">Detta tar bort både klient- och serverregler.</span><span class="sxs-lookup"><span data-stu-id="5fd17-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="5fd17-113">Alla regler för alla konton i Outlook-profilen tas bort.</span><span class="sxs-lookup"><span data-stu-id="5fd17-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="5fd17-114">Det här kommandot dokumenteras ytterligare i artikeln Kommandoradsväxlar.</span><span class="sxs-lookup"><span data-stu-id="5fd17-114">This command is further documented in the Command-line switches  article.</span></span>