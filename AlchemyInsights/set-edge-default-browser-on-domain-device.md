---
title: Ange Microsoft Edge som standardwebbläsare på en domän ansluten enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491877"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="ef6e1-102">Ange Microsoft Edge som standardwebbläsare på en domän ansluten enhet</span><span class="sxs-lookup"><span data-stu-id="ef6e1-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="ef6e1-103">Ange Microsoft Edge som standardwebbläsare:</span><span class="sxs-lookup"><span data-stu-id="ef6e1-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="ef6e1-104">[Skapa en konfigurationsfil för standardassociationer](https://go.microsoft.com/fwlink/?linkid=2132437) och lagra den lokalt eller på en nätverksresurs.</span><span class="sxs-lookup"><span data-stu-id="ef6e1-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="ef6e1-105">Öppna grupprincipredigeraren och gå sedan till Administrativa mallar för  >  **datorkonfiguration**  >  **Windows-komponenter**  >  **Utforskaren.**</span><span class="sxs-lookup"><span data-stu-id="ef6e1-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="ef6e1-106">Välj **Ange en konfigurationsfil för standardassociationer**.</span><span class="sxs-lookup"><span data-stu-id="ef6e1-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="ef6e1-107">Välj **Principinställning** och välj sedan **Aktiverad**.</span><span class="sxs-lookup"><span data-stu-id="ef6e1-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="ef6e1-108">Under **Alternativ** anger du platsen för konfigurationsfilen för standardassociationer och väljer **sedan OK.**</span><span class="sxs-lookup"><span data-stu-id="ef6e1-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
