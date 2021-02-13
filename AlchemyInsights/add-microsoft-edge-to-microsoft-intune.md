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
# <a name="add-microsoft-edge-to-microsoft-intune"></a>Lägga till Microsoft Edge i Microsoft Intune

För att kunna distribuera, konfigurera, övervaka och skydda Microsoft Edge för Windows 10 måste du först lägga till den i Microsoft Intune.

> [!IMPORTANT]
- Intune har stöd för Microsoft Edge 77 och senare versioner.
- Intune identifierar alla befintliga installationer av Microsoft Edge.
- Om Microsoft Edge installeras i användarsammanhang skriver systeminstallationen över installationen i användarsammanhang.
- Om Microsoft Edge installerats i systemsammanhang rapporteras installationen.
- Förinstallerade Microsoft Edge 77 och senare versioner, för alla kanaler i användarsammanhang, skrivs över med Microsoft Edge installerat i systemsammanhang.

**Förutsättningar**

Windows 10 version 1709 eller senare versioner

**Steg för att lägga till Edge i Intune**

1. [Konfigurera appen i Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
2. [Konfigurera appinformationen.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
3. [Konfigurera appinställningarna.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
4. [Välj omfattningstaggarna (valfritt).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
5. [Lägg till programmet.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)

Mer hjälp finns i [Felsökning.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)




