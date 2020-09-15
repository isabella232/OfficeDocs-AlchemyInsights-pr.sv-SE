---
title: 'Fel: reglerna på den här datorn stämmer inte överens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690981"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="454a9-102">Fel: reglerna på den här datorn stämmer inte överens</span><span class="sxs-lookup"><span data-stu-id="454a9-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="454a9-103">Om du vill se uppdaterad status för det här kända problemet läser [du reglerna på den här datorn stämmer inte överens med reglerna för Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="454a9-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="454a9-104">Outlook-teamet har implementerat en korrigering i version 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="454a9-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="454a9-105">Korrigeringen är redan i Insider – snabbt och kommer att gå till månads kanal i 2020 i sent juni.</span><span class="sxs-lookup"><span data-stu-id="454a9-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="454a9-106">När du har den fasta versionen kan du få meddelandet "vilka regler vill du behålla" en sista gång.</span><span class="sxs-lookup"><span data-stu-id="454a9-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="454a9-107">Välj server när du uppmanas till det och gå tillbaka till Outlook och återaktivera eventuella regler som inaktiverats.</span><span class="sxs-lookup"><span data-stu-id="454a9-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="454a9-108">När korrigeringen är tillgänglig kan du använda följande lösning:</span><span class="sxs-lookup"><span data-stu-id="454a9-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="454a9-109">**Lösning**: problemet har uppstått i de senaste rapporterna för dem som bara har skapat klient regler i Outlook-skrivbordet.</span><span class="sxs-lookup"><span data-stu-id="454a9-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="454a9-110">Om du fortsätter med problemet kan du överväga att ta bort reglerna och sedan skapa och redigera regler endast i OWA (Outlook Web App) tills problemet är löst.</span><span class="sxs-lookup"><span data-stu-id="454a9-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="454a9-111">Om du inte kan ta bort reglerna manuellt kan du köra ett Outlook-kommando när du startar Outlook genom att köra Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="454a9-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="454a9-112">Detta tar bort både klient-och Server reglerna.</span><span class="sxs-lookup"><span data-stu-id="454a9-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="454a9-113">Alla regler för alla konton i Outlook-profilen tas bort.</span><span class="sxs-lookup"><span data-stu-id="454a9-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="454a9-114">Det här kommandot dokumenteras också i artikeln kommando rads växlar.</span><span class="sxs-lookup"><span data-stu-id="454a9-114">This command is further documented in the Command-line switches article.</span></span>

