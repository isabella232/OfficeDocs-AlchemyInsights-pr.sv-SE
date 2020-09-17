---
title: Om du dubbelklickar på en Office-fil öppnas inte den
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812097"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="abdec-102">Om du dubbelklickar på en Office-fil öppnas inte den</span><span class="sxs-lookup"><span data-stu-id="abdec-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="abdec-103">När du dubbelklickar på en Office-fil kan programmet öppnas, men själva filen öppnas inte.</span><span class="sxs-lookup"><span data-stu-id="abdec-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="abdec-104">Eller så får du fel meddelandet "ett problem uppstod när du skickade kommandot till programmet".</span><span class="sxs-lookup"><span data-stu-id="abdec-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="abdec-105">Det finns många orsaker till det, men de två vanligaste lösningarna är:</span><span class="sxs-lookup"><span data-stu-id="abdec-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="abdec-106">I Excel kontrollerar du att DDE-alternativet inte är markerat.</span><span class="sxs-lookup"><span data-stu-id="abdec-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="abdec-107">Du kan hitta alternativet genom att skapa en ny arbets bok och sedan välja **alternativ för > > Avancerat**.</span><span class="sxs-lookup"><span data-stu-id="abdec-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="abdec-108">I avsnittet **Allmänt** avmarkerar du **Ignorera andra program som använder DDE (Dynamic Data Exchange)**.</span><span class="sxs-lookup"><span data-stu-id="abdec-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="abdec-109">Kör en online-reparation för att återställa standardinställningarna.</span><span class="sxs-lookup"><span data-stu-id="abdec-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="abdec-110">Klicka på Start-knappen i Windows och Sök efter "kontroll panelen".</span><span class="sxs-lookup"><span data-stu-id="abdec-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="abdec-111">Öppna **kontroll panelen**och gå till **program > program och funktioner**.</span><span class="sxs-lookup"><span data-stu-id="abdec-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="abdec-112">Högerklicka sedan på **Microsoft Office [version]** och välj **ändra > online-reparation**.</span><span class="sxs-lookup"><span data-stu-id="abdec-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="abdec-113">Om ingen av dessa lösningar fungerar, en mer fullständig lista över lösningar finns i Support artikeln kan du [dubbelklicka på en Office-fil för att öppna den](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="abdec-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
