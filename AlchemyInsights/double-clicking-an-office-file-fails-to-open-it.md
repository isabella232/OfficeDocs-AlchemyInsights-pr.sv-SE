---
title: Det går inte att öppna den genom att dubbelklicka på en Office-fil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573601"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="84934-102">Det går inte att öppna den genom att dubbelklicka på en Office-fil</span><span class="sxs-lookup"><span data-stu-id="84934-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="84934-103">När du har dubbelklickat på en Office-fil kan programmet öppnas, men själva filen öppnas inte.</span><span class="sxs-lookup"><span data-stu-id="84934-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="84934-104">Eller så kan du få felet: "Det var ett problem att skicka kommandot till programmet."</span><span class="sxs-lookup"><span data-stu-id="84934-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="84934-105">Det finns många orsaker till detta, men de två vanligaste lösningarna är:</span><span class="sxs-lookup"><span data-stu-id="84934-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="84934-106">Inifrån Excel kontrollerar du att Alternativet DDE är avmarkerat.</span><span class="sxs-lookup"><span data-stu-id="84934-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="84934-107">Alternativet kan hittas genom att skapa en ny arbetsbok och sedan välja **Arkiv > Alternativ > Avancerat**.</span><span class="sxs-lookup"><span data-stu-id="84934-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="84934-108">Avmarkera **ignorera andra program som använder DDE (Dynamic Data Exchange) i**avsnittet **Allmänt** .</span><span class="sxs-lookup"><span data-stu-id="84934-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="84934-109">Kör en onlinereparation för att återställa standardinställningarna.</span><span class="sxs-lookup"><span data-stu-id="84934-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="84934-110">Klicka på Start-knappen i Windows och sök efter "Kontrollpanelen".</span><span class="sxs-lookup"><span data-stu-id="84934-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="84934-111">Öppna **Kontrollpanelen**och gå till **Program > program och funktioner**.</span><span class="sxs-lookup"><span data-stu-id="84934-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="84934-112">Högerklicka sedan på **Microsoft Office [Version]** och välj **Ändra > Online Repair**.</span><span class="sxs-lookup"><span data-stu-id="84934-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="84934-113">Om ingen av dessa lösningar fungerar kan en mer komplett lista över lösningar hittas i supportartikeln, [Dubbelklicka på en Office-fil kan inte öppna den](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="84934-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
