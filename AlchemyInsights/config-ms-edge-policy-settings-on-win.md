---
title: Konfigurera principinställningar för Microsoft Edge i Windows
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
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402393"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="fe720-102">Konfigurera principinställningar för Microsoft Edge i Windows</span><span class="sxs-lookup"><span data-stu-id="fe720-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="fe720-103">Om du vill konfigurera principinställningar och hanterade uppdateringar för Microsoft Edge använder du grupprincipobjekt (GPOs).</span><span class="sxs-lookup"><span data-stu-id="fe720-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="fe720-104">Du kan också etablera princip via registret. Detta är lämpligt för (1) Windows-enheter som är anslutna till en Microsoft Active Directory-domän och för (2) Windows 10 Pro- och Enterprise-instanser som har registrerats för enhetshantering i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="fe720-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="fe720-105">Om du vill konfigurera Microsoft Edge med hjälp av GPOs gör du följande:</span><span class="sxs-lookup"><span data-stu-id="fe720-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="fe720-106">Gå till den centrala lagringslistan för grupprinciper i Active Directory-domänen, eller till mallmappen Principdefinition på enskilda datorer, och installera alla administrativa mallar som lägger till regler och inställningar för Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="fe720-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="fe720-107">Konfigurera de specifika principer som du vill ange.</span><span class="sxs-lookup"><span data-stu-id="fe720-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="fe720-108">Mer information finns i Konfigurera [principinställningar för Microsoft Edge i Windows.](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="fe720-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
