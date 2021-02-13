---
title: Lägga till Microsoft Edge i Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194577"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="0782f-102">Lägga till Microsoft Edge i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0782f-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="0782f-103">För att kunna distribuera, konfigurera, övervaka och skydda Microsoft Edge för Windows 10 måste du först lägga till den i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0782f-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="0782f-104">Intune har stöd för Microsoft Edge 77 och senare versioner.</span><span class="sxs-lookup"><span data-stu-id="0782f-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="0782f-105">Intune identifierar alla befintliga installationer av Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="0782f-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="0782f-106">Om Microsoft Edge installeras i användarsammanhang skriver systeminstallationen över installationen i användarsammanhang.</span><span class="sxs-lookup"><span data-stu-id="0782f-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="0782f-107">Om Microsoft Edge installerats i systemsammanhang rapporteras installationen.</span><span class="sxs-lookup"><span data-stu-id="0782f-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="0782f-108">Förinstallerade Microsoft Edge 77 och senare versioner, för alla kanaler i användarsammanhang, skrivs över med Microsoft Edge installerat i systemsammanhang.</span><span class="sxs-lookup"><span data-stu-id="0782f-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="0782f-109">**Förutsättningar**</span><span class="sxs-lookup"><span data-stu-id="0782f-109">**Prerequisite**</span></span>

<span data-ttu-id="0782f-110">Windows 10 version 1709 eller senare versioner</span><span class="sxs-lookup"><span data-stu-id="0782f-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="0782f-111">**Steg för att lägga till Edge i Intune**</span><span class="sxs-lookup"><span data-stu-id="0782f-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="0782f-112">[Konfigurera appen i Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="0782f-113">[Konfigurera appinformationen.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="0782f-114">[Konfigurera appinställningarna.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="0782f-115">[Välj omfattningstaggarna (valfritt).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="0782f-116">[Lägg till programmet.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="0782f-117">Mer hjälp finns i [Felsökning.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="0782f-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




