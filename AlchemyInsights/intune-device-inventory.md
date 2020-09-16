---
title: Enhets inventering i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667896"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="c886e-102">Enhets inventering i Intune</span><span class="sxs-lookup"><span data-stu-id="c886e-102">Intune Device Inventory</span></span>

<span data-ttu-id="c886e-103">Med enheten enheter får administratören en inblick i enheter under hantering i Intune per enhet.</span><span class="sxs-lookup"><span data-stu-id="c886e-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="c886e-104">Informationen som visas är: maskin vara, upptäckta program, enhetens kompatibilitetsstatus och status för enhets konfiguration.</span><span class="sxs-lookup"><span data-stu-id="c886e-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="c886e-105">Lager data för hård vara och upptäckta program samlas in på sju dagar.</span><span class="sxs-lookup"><span data-stu-id="c886e-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="c886e-106">Vilka program och specifika delar av maskin varan som rapporteras varierar beroende på enhetens operativ system och om enheten är personligen eller ägda.</span><span class="sxs-lookup"><span data-stu-id="c886e-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="c886e-107">Mer information finns i [Se enhets detaljer i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="c886e-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="c886e-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="c886e-108">**FAQ**</span></span>

<span data-ttu-id="c886e-109">F: Jag får inte en fullständig inventering av program som finns på Intune-registrerade Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="c886e-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="c886e-110">Varför inte?</span><span class="sxs-lookup"><span data-stu-id="c886e-110">Why not?</span></span>

<span data-ttu-id="c886e-111">A: i det här fallet visas bara moderna appar för Windows 10-datorer som identifieras som företags enheter.</span><span class="sxs-lookup"><span data-stu-id="c886e-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="c886e-112">Intune samlar inte in information om Win32-program som är installerade på dessa enheter.</span><span class="sxs-lookup"><span data-stu-id="c886e-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="c886e-113">F: Varför hämtas inte telefonnummer från alla enheter?</span><span class="sxs-lookup"><span data-stu-id="c886e-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="c886e-114">A: telefoner kategoriserade som företags enheter i Intune identifieras inte med deras fullständiga telefonnummer när du till exempel kör en inventerings rapport för mobila enheter.</span><span class="sxs-lookup"><span data-stu-id="c886e-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="c886e-115">Fasta enheter telefonnummer är alltid delvis maskerade med asterisker (\* \* \* \*) och bara visa de fyra sista siffrorna.</span><span class="sxs-lookup"><span data-stu-id="c886e-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>