---
title: Intune Win32 app Deployment
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461994"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="2e69a-102">Intune Win32 app Deployment</span><span class="sxs-lookup"><span data-stu-id="2e69a-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="2e69a-103">Microsoft Intune tillåter Win32-program, inklusive men inte begränsat till MSI och. EXE för att distribueras till Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="2e69a-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="2e69a-104">Den distributions funktion som används kräver att det finns ett Intune Management Extension (IME) på mål enheten.</span><span class="sxs-lookup"><span data-stu-id="2e69a-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="2e69a-105">IME installeras automatiskt som ett resultat av att ett PowerShell-skript eller en Win32-tillämpning distribueras till en användare/enhet.</span><span class="sxs-lookup"><span data-stu-id="2e69a-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="2e69a-106">Det finns också en uppsättning förutsättningar som måste uppfyllas för att du ska kunna distribuera Win32-appar som inkluderar:</span><span class="sxs-lookup"><span data-stu-id="2e69a-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="2e69a-107">Plattformar som stöds: Windows 10 version 1607 eller senare (Enterprise, Pro och Education-version).</span><span class="sxs-lookup"><span data-stu-id="2e69a-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="2e69a-108">Arkitektur som stöds: x86 och x64.</span><span class="sxs-lookup"><span data-stu-id="2e69a-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="2e69a-109">Enhets hantering: AAD-uppkopplad och automatisk registrering (inklusive hybrid domän ansluten och automatisk registrering via grup princip).</span><span class="sxs-lookup"><span data-stu-id="2e69a-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="2e69a-110">Format för programpaket:. **intunewin**  -fil som skapats av [Microsoft Win32-innehålls förberedelse verktyget](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="2e69a-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="2e69a-111">Begränsat</span><span class="sxs-lookup"><span data-stu-id="2e69a-111">Limitations:</span></span>
    - <span data-ttu-id="2e69a-112">Maximal storlek: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="2e69a-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="2e69a-113">Arkitektur som inte stöds: armar.</span><span class="sxs-lookup"><span data-stu-id="2e69a-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="2e69a-114">Granska dokumentet "[Lägg till, tilldela och övervaka en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" för information som rör dessa steg.</span><span class="sxs-lookup"><span data-stu-id="2e69a-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="2e69a-115">Information om hur du felsöker program distributioner i Windows, inklusive Win32-appar, kan granskas i följande dokument</span><span class="sxs-lookup"><span data-stu-id="2e69a-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="2e69a-116">Felsöka problem med programinstallation</span><span class="sxs-lookup"><span data-stu-id="2e69a-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="2e69a-117">Felsöka Win32-appar</span><span class="sxs-lookup"><span data-stu-id="2e69a-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)