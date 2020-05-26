---
title: Köra Windows Minnesdiagnostik i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358293"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="7394e-102">Köra Windows Minnesdiagnostik i Windows 10</span><span class="sxs-lookup"><span data-stu-id="7394e-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="7394e-103">Om Windows och appar på datorn kraschar, fryser eller agerar på ett instabilt sätt kan det vara problem med datorns minne (RAM).</span><span class="sxs-lookup"><span data-stu-id="7394e-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="7394e-104">Du kan köra Windows Memory Diagnostic för att söka efter problem med datorns RAM.You can run the Windows Memory Diagnostic to check for problems with the PC's RAM.</span><span class="sxs-lookup"><span data-stu-id="7394e-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="7394e-105">Skriv **minnesdiagnostik**i sökrutan i Aktivitetsfältet och välj sedan **Windows Minnesdiagnostik**.</span><span class="sxs-lookup"><span data-stu-id="7394e-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="7394e-106">För att köra diagnostiken måste datorn startas om.</span><span class="sxs-lookup"><span data-stu-id="7394e-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="7394e-107">Du har möjlighet att starta om omedelbart (spara ditt arbete och stäng öppna dokument och e-post först), eller schemalägga diagnostiken så att den körs automatiskt nästa gång datorn startas om:</span><span class="sxs-lookup"><span data-stu-id="7394e-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostik av Windows-minne](media/windows-memory-diagnostic.png)

<span data-ttu-id="7394e-109">När datorn startas om körs **Windows Minnesdiagnostikverktyg** automatiskt.</span><span class="sxs-lookup"><span data-stu-id="7394e-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="7394e-110">Status och förlopp visas när diagnostiken körs, och du har möjlighet att avbryta diagnostiken genom att trycka på **ESC-tangenten** på tangentbordet.</span><span class="sxs-lookup"><span data-stu-id="7394e-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="7394e-111">När diagnostiken är klar startar Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="7394e-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="7394e-112">Omedelbart efter omstarten visas ett meddelande (bredvid **åtgärdscenterikonen** i Aktivitetsfältet) när skrivbordet visas (bredvid åtgärdscenterikonen i Aktivitetsfältet) för att ange om några minnesfel hittades.</span><span class="sxs-lookup"><span data-stu-id="7394e-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="7394e-113">Ett exempel:</span><span class="sxs-lookup"><span data-stu-id="7394e-113">For example:</span></span>

<span data-ttu-id="7394e-114">Här är ikonen i Åtgärdscenter:</span><span class="sxs-lookup"><span data-stu-id="7394e-114">Here's the Action Center icon:</span></span> ![Ikon för Åtgärdscenter](media/action-center-icon.png) 

<span data-ttu-id="7394e-116">Och ett exempel meddelande:</span><span class="sxs-lookup"><span data-stu-id="7394e-116">And a sample notification:</span></span> ![Inga minnesfel](media/no-memory-errors.png)

<span data-ttu-id="7394e-118">Om du missade meddelandet kan du välja **ikonen Åtgärdscenter** i Aktivitetsfältet för att visa **Åtgärdscenter** och se en rullningsbar lista med meddelanden.</span><span class="sxs-lookup"><span data-stu-id="7394e-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="7394e-119">Om du vill granska detaljerad information skriver du **händelsen** i sökrutan i Aktivitetsfältet och väljer sedan **Loggboken**.</span><span class="sxs-lookup"><span data-stu-id="7394e-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="7394e-120">I **loggbokens**vänstra fönster navigerar du till **Windows-loggar > System**.</span><span class="sxs-lookup"><span data-stu-id="7394e-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="7394e-121">I det högra fönstret söker du ned listan medan du tittar på kolumnen **Källa** tills du ser händelser med källvärde **Minnesdiagnostik-resultat**.</span><span class="sxs-lookup"><span data-stu-id="7394e-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="7394e-122">Markera varje sådan händelse och se resultatinformationen i rutan under fliken **Allmänt** under listan.</span><span class="sxs-lookup"><span data-stu-id="7394e-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
