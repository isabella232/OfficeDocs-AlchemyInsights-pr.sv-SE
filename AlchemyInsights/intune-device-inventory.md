---
title: Intune-enhetslager
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440478"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="7e4ac-102">Intune-enhetslager</span><span class="sxs-lookup"><span data-stu-id="7e4ac-102">Intune Device Inventory</span></span>

<span data-ttu-id="7e4ac-103">Bladet Enheter ger administratören insikt i enheter under hantering i Intune per enhet.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="7e4ac-104">Informationen som visas innehåller: Maskinvara, identifierade program, enhetsefterlevnadstillstånd och enhetskonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="7e4ac-105">Inventeringsdata för maskinvara och identifierade program samlas in på en sjudagarscykel.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="7e4ac-106">Programmen och specifika delar av maskinvara som rapporteras skiljer sig åt beroende på enhetens operativsystem och om enheten ägs personligen eller i företaget.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="7e4ac-107">Mer information finns [i Se enhetsinformation i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="7e4ac-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="7e4ac-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="7e4ac-108">**FAQ**</span></span>

<span data-ttu-id="7e4ac-109">F: Jag får inte en fullständig inventeringslista över program som finns på Intune-registrerade Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="7e4ac-110">Varför inte?</span><span class="sxs-lookup"><span data-stu-id="7e4ac-110">Why not?</span></span>

<span data-ttu-id="7e4ac-111">S: För närvarande visas endast moderna appar för Windows 10-datorer som identifieras som företagsenheter.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="7e4ac-112">Intune samlar inte in information om Win32-appar som är installerade på dessa enheter.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="7e4ac-113">F: Varför samlas inte telefonnummer in från alla enheter?</span><span class="sxs-lookup"><span data-stu-id="7e4ac-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="7e4ac-114">S: Telefoner som kategoriseras som företagsenheter i Intune identifieras inte med sitt fullständiga telefonnummer när du till exempel kör en inventeringsrapport för mobila enheter.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="7e4ac-115">Telefonnummer för bring-you-own-enhet är alltid delvis maskerade med asterisker (\*\*\*\*) och visar bara de fyra sista siffrorna.</span><span class="sxs-lookup"><span data-stu-id="7e4ac-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>