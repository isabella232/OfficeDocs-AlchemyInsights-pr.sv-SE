---
title: Kör Windows Minnesdiagnostik i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826685"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="19cba-102">Kör Windows Minnesdiagnostik i Windows 10</span><span class="sxs-lookup"><span data-stu-id="19cba-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="19cba-103">Om Windows och appar på din dator kraschar, fryser eller fungerar instabilt kan du ha problem med datorns minne ..</span><span class="sxs-lookup"><span data-stu-id="19cba-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="19cba-104">Du kan köra Windows Minnesdiagnostik för att söka efter problem med datorns RAM-minne.</span><span class="sxs-lookup"><span data-stu-id="19cba-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="19cba-105">Skriv minnesdiagnostik i sökrutan i **Aktivitetsfältet och** välj sedan **Windows minnesdiagnostik.**</span><span class="sxs-lookup"><span data-stu-id="19cba-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="19cba-106">För att kunna köra diagnostiken måste datorn starta om.</span><span class="sxs-lookup"><span data-stu-id="19cba-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="19cba-107">Du kan starta om direkt (spara ditt arbete och stäng öppna dokument och e-postmeddelanden först) eller schemalägga diagnostiken så att den körs automatiskt nästa gång datorn startar om:</span><span class="sxs-lookup"><span data-stu-id="19cba-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Minnesdiagnostik](media/windows-memory-diagnostic.png)

<span data-ttu-id="19cba-109">När datorn startas om körs **windows minnesdiagnostikverktyget** automatiskt.</span><span class="sxs-lookup"><span data-stu-id="19cba-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="19cba-110">Status och förlopp visas medan diagnostiken körs och du kan välja att avbryta diagnostiken genom att trycka på **ESC** på tangentbordet.</span><span class="sxs-lookup"><span data-stu-id="19cba-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="19cba-111">När diagnostiken är klar startar Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="19cba-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="19cba-112">Omedelbart efter omstarten, när skrivbordet visas, visas  ett meddelande (bredvid ikonen för Åtgärdscenter i Aktivitetsfältet) som anger om några minnesfel hittades.</span><span class="sxs-lookup"><span data-stu-id="19cba-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="19cba-113">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="19cba-113">For example:</span></span>

<span data-ttu-id="19cba-114">Här är ikonen för Åtgärdscenter:</span><span class="sxs-lookup"><span data-stu-id="19cba-114">Here's the Action Center icon:</span></span> ![Ikon för Åtgärdscenter](media/action-center-icon.png) 

<span data-ttu-id="19cba-116">Och ett exempelmeddelande:</span><span class="sxs-lookup"><span data-stu-id="19cba-116">And a sample notification:</span></span> ![Inga minnesfel](media/no-memory-errors.png)

<span data-ttu-id="19cba-118">Om du missade meddelandet kan  du välja ikonen för Åtgärdscenter i Aktivitetsfältet för att visa **Åtgärdscenter** och se en rullningsbar lista med meddelanden.</span><span class="sxs-lookup"><span data-stu-id="19cba-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="19cba-119">Om du vill granska detaljerad information **skriver** du händelsen i sökrutan i Aktivitetsfältet och väljer sedan **Loggboken**.</span><span class="sxs-lookup"><span data-stu-id="19cba-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="19cba-120">I det **vänstra fönstret** i Loggboken går du till **Windows-loggar > System.**</span><span class="sxs-lookup"><span data-stu-id="19cba-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="19cba-121">I fönstret till höger söker du nedåt i  listan medan du tittar på kolumnen Källa, tills du ser händelser med källvärdet **Minnesdiagnostics-Resultat.**</span><span class="sxs-lookup"><span data-stu-id="19cba-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="19cba-122">Markera varje sådan händelse och se resultatinformationen i rutan under **fliken** Allmänt under listan.</span><span class="sxs-lookup"><span data-stu-id="19cba-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
