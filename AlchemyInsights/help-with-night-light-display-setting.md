---
title: Hjälp med inställningen för nattlampan
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405182"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="61d9a-102">Hjälp med inställningen för nattlampan</span><span class="sxs-lookup"><span data-stu-id="61d9a-102">Help with the night light display setting</span></span>

<span data-ttu-id="61d9a-103">Mer information om bildskärmsinställningar för natttid finns [i Ställ in bildskärmen på natttid i Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="61d9a-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="61d9a-104">Om alternativen för nattljus är nedtonade i Inställningar kontrollerar du bildskärmsdrivrutinen:</span><span class="sxs-lookup"><span data-stu-id="61d9a-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="61d9a-105">Klicka på sökrutan i Aktivitetsfältet, **skriv Enhetshanteraren** och välj **sedan Enhetshanteraren** i sökresultatet.</span><span class="sxs-lookup"><span data-stu-id="61d9a-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="61d9a-106">Expandera **Bildskärmskort**.</span><span class="sxs-lookup"><span data-stu-id="61d9a-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="61d9a-107">Funktionen nattlampan är tyvärr inte tillgänglig om enheten använder en DisplayLink-drivrutin eller en grundläggande bildskärmsdrivrutin.</span><span class="sxs-lookup"><span data-stu-id="61d9a-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="61d9a-108">Nattlampan använder den senaste grafiktekniken så du kan behöva uppdatera bildskärmsdrivrutinen:</span><span class="sxs-lookup"><span data-stu-id="61d9a-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="61d9a-109">Sök efter uppdateringar genom att gå till **Starta**  >  **inställningar Uppdatering**&  >  **säkerhetsuppdatering** Windows  >  **Update** Sök  >  **efter uppdateringar.**</span><span class="sxs-lookup"><span data-stu-id="61d9a-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="61d9a-110">ELLER</span><span class="sxs-lookup"><span data-stu-id="61d9a-110">OR</span></span>

- <span data-ttu-id="61d9a-111">Gå till maskinvarutillverkarens supportwebbplats och ladda ned och installera de senaste bildskärmsdrivrutinerna manuellt.</span><span class="sxs-lookup"><span data-stu-id="61d9a-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="61d9a-112">Återställa nattlampan i registret</span><span class="sxs-lookup"><span data-stu-id="61d9a-112">Reset night light in the registry</span></span>

<span data-ttu-id="61d9a-113">Om det inte fungerar att uppdatera visningsdrivrutinen kan du behöva återställa nattlampan i registret.</span><span class="sxs-lookup"><span data-stu-id="61d9a-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="61d9a-114">**Varning!** Det här steget för felsökning rekommenderas endast för avancerade användare.</span><span class="sxs-lookup"><span data-stu-id="61d9a-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="61d9a-115">Om du ändrar i registret på fel sätt kan det orsaka allvarliga problem.</span><span class="sxs-lookup"><span data-stu-id="61d9a-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="61d9a-116">För ytterligare skydd bör du skydda registret innan du ändrar det så att du kan återställa det om det uppstår problem.</span><span class="sxs-lookup"><span data-stu-id="61d9a-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="61d9a-117">Skriv **regedit** i sökrutan och välj sedan **Registereditorn** i sökresultatet.</span><span class="sxs-lookup"><span data-stu-id="61d9a-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="61d9a-118">Gå till följande registernyckel:</span><span class="sxs-lookup"><span data-stu-id="61d9a-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="61d9a-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="61d9a-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="61d9a-120">Exportera och ta sedan bort följande undernyckel:$$windows.data.bluelightreduktion.bluelightreduktionsstate</span><span class="sxs-lookup"><span data-stu-id="61d9a-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="61d9a-121">Exportera och ta sedan bort följande undernyckel:$$windows.data.bluelightreduktion.settings</span><span class="sxs-lookup"><span data-stu-id="61d9a-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="61d9a-122">Starta om Windows och kontrollera om alternativen för nattlampan är tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="61d9a-122">Restart Windows and verify if the night light options are available.</span></span>


