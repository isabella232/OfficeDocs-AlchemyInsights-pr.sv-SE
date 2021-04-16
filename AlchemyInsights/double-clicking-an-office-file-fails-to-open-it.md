---
title: Det går inte att öppna en Office-fil när du dubbelklickar på den
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814823"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="bc78d-102">Det går inte att öppna en Office-fil när du dubbelklickar på den</span><span class="sxs-lookup"><span data-stu-id="bc78d-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="bc78d-103">När du dubbelklickat på en Office-fil kan programmet öppnas men själva filen öppnas inte.</span><span class="sxs-lookup"><span data-stu-id="bc78d-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="bc78d-104">Eller så kan du få felmeddelandet: "Ett problem uppstod när kommandot skulle skickas till programmet."</span><span class="sxs-lookup"><span data-stu-id="bc78d-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="bc78d-105">Det finns många orsaker till detta, men de två vanligaste lösningarna är:</span><span class="sxs-lookup"><span data-stu-id="bc78d-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="bc78d-106">Kontrollera att DDE-alternativet är avmarkerat i Excel.</span><span class="sxs-lookup"><span data-stu-id="bc78d-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="bc78d-107">Du hittar alternativet genom att skapa en ny arbetsbok och sedan välja **Arkiv eller > Alternativ > Avancerat.**</span><span class="sxs-lookup"><span data-stu-id="bc78d-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="bc78d-108">I avsnittet **Allmänt** avmarkerar du **ignorera andra program som använder DDE (Dynamic Data Exchange).**</span><span class="sxs-lookup"><span data-stu-id="bc78d-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="bc78d-109">Kör en onlinereparation för att återställa standardinställningarna.</span><span class="sxs-lookup"><span data-stu-id="bc78d-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="bc78d-110">Klicka på Start-knappen i Windows och sök efter "Kontrollpanelen".</span><span class="sxs-lookup"><span data-stu-id="bc78d-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="bc78d-111">Öppna **Kontrollpanelen och** gå till Program **för > Program och funktioner**.</span><span class="sxs-lookup"><span data-stu-id="bc78d-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="bc78d-112">Högerklicka sedan på **Microsoft Office [version]** och välj **Ändra > Onlinereparation**.</span><span class="sxs-lookup"><span data-stu-id="bc78d-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="bc78d-113">Om ingen av de här lösningarna fungerar kan du hitta en mer fullständig lista med lösningar i hjälpartikeln, så öppnas den inte när du dubbelklickar [på en Office-fil.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="bc78d-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
