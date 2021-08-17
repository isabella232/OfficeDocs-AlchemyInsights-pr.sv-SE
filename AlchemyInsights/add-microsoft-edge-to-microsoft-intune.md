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
ms.openlocfilehash: 7cfc2279acf18a7cb6fab89befc8ef1ccc7a4be7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315142"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a>Lägga till Microsoft Edge i Microsoft Intune

För att kunna distribuera, konfigurera, övervaka och skydda Microsoft Edge för Windows 10 måste du först lägga till det i Microsoft Intune.

> **Viktigt:**
- Intune har stöd för Microsoft Edge 77 och senare versioner.
- Intune identifierar alla befintliga installationer av Microsoft Edge.
- Om Microsoft Edge installeras i användarsammanhang skriver en systeminstallation över installationen i användarkontext.
- Om Microsoft Edge installerats i systemsammanhang rapporteras installationens framgång.
- Förinstallerade Microsoft Edge 77 och senare versioner, för alla kanaler i användarsammanhang, skrivs över med Microsoft Edge installerat i systemsammanhang.

**Krav**

Windows 10 version 1709 eller senare versioner

**Steg för att lägga till Edge i Intune**

1. [Konfigurera appen i Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
2. [Konfigurera appinformationen](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
3. [Konfigurera appinställningarna](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
4. [Välj omfattningstaggar (valfritt)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).
5. [Lägg till appen](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).

Mer hjälp finns i [Felsökning](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).




