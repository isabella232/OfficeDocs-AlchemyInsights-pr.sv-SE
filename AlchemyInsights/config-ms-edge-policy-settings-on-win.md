---
title: Konfigurera princip inställningar för Microsoft Edge i Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583746"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="4f447-102">Konfigurera princip inställningar för Microsoft Edge i Windows</span><span class="sxs-lookup"><span data-stu-id="4f447-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="4f447-103">Om du vill konfigurera princip inställningar och hanterade uppdateringar för Microsoft Edge använder du grup princip objekt (GPO).</span><span class="sxs-lookup"><span data-stu-id="4f447-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="4f447-104">Du kan också etablera princip via registret. Det här är lämpligt för (1) Windows-enheter som är anslutna till en Microsoft Active Directory-domän och för (2) Windows 10 Pro-och Enterprise-instanser registrerade för enhets hantering i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4f447-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="4f447-105">Om du vill konfigurera Microsoft Edge med hjälp av grup princip objekt gör du följande:</span><span class="sxs-lookup"><span data-stu-id="4f447-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="4f447-106">Till Central arkivet för grup princip i din Active Directory-domän, eller till mappen princip definitions mal len på enskilda datorer, installerar du alla administrativa mallar som lägger till regler och inställningar för Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4f447-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="4f447-107">Konfigurera de principer du vill ange.</span><span class="sxs-lookup"><span data-stu-id="4f447-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="4f447-108">Mer information finns i [Konfigurera inställningar för Microsoft Edge-principer i Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="4f447-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
