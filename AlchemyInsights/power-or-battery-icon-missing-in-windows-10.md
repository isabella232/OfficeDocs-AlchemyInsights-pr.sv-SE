---
title: Ikonen för ström eller batteriet saknas i Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790566"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="1dc35-102">Ikonen för ström eller batteriet saknas i Windows 10</span><span class="sxs-lookup"><span data-stu-id="1dc35-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="1dc35-103">Om din Windows 10-enhet har ett batteri (t.ex. en bärbar dator, surfplatta eller en dator ansluten via USB till en UPS) visas vanligtvis en ikon för ström eller batteri i aktivitetsfältet nära klockan, till exempel:</span><span class="sxs-lookup"><span data-stu-id="1dc35-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Batteriets ikon](media/battery-icon.png)

<span data-ttu-id="1dc35-105">Om den här ikonen inte visas kan den vara dold:</span><span class="sxs-lookup"><span data-stu-id="1dc35-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="1dc35-106">Gå till **[Inställningar > Anpassning > Aktivitetsfältet](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="1dc35-107">I meddelandefältet klickar du på **Välj vilka ikoner som ska visas i Aktivitetsfältet**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="1dc35-108">Leta sedan efter objektet för **Ström** i listan och ändra inställningen till **På**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Visa ikon för Ström i Aktivitetsfältet](media/power-icon-on.png)

<span data-ttu-id="1dc35-110">**Felsökning**</span><span class="sxs-lookup"><span data-stu-id="1dc35-110">**Troubleshooting**</span></span>

<span data-ttu-id="1dc35-111">Om du följde anvisningarna ovan och knappen för **Ström** är nedtonad eller inte visas går du till sökrutan i Aktivitetsfältet och skriver in **Enhetshanteraren**, välj sedan **Enhetshanteraren** i resultatlistan.</span><span class="sxs-lookup"><span data-stu-id="1dc35-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="1dc35-112">Via **Batterier** högerklickar du på enhetens batteri, klicka på **Inaktivera** och sedan på **Ja**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="1dc35-113">Vänta några sekunder och högerklicka sedan på batteriet och klicka på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="1dc35-114">Starta sedan om enheten.</span><span class="sxs-lookup"><span data-stu-id="1dc35-114">Then restart your device.</span></span>

<span data-ttu-id="1dc35-115">Om du följde anvisningarna ovan men ikonen för batteriet visas inte i aktivitetsfältet går du till sökrutan i Aktivitetsfältet och skriver in **Aktivitetshanteraren**, klicka sedan på **Aktivitetshanteraren** i resultatlistan.</span><span class="sxs-lookup"><span data-stu-id="1dc35-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="1dc35-116">På fliken **Processer** under **Namn** högerklickar du på **Utforskaren** och klickar sedan på **Starta om**.</span><span class="sxs-lookup"><span data-stu-id="1dc35-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
