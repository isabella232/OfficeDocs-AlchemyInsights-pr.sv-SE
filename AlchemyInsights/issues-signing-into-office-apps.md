---
title: Problem med att logga in på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709124"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="1c5d1-102">Åtgärda meddelandet "Din dators modul för betrodd plattform fungerar inte korrekt" i Microsoft 365-programmen</span><span class="sxs-lookup"><span data-stu-id="1c5d1-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="1c5d1-103">Lös problemet genom att prova med följande:</span><span class="sxs-lookup"><span data-stu-id="1c5d1-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="1c5d1-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="1c5d1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="1c5d1-105">[Ta bort Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) med Hjälp av Autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="1c5d1-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="1c5d1-106">**Obs!** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="1c5d1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="1c5d1-107">(Exempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="1c5d1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="1c5d1-108">Prova [återställningsprocessen för användare för](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) att åtgärda TPM-fel (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="1c5d1-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="1c5d1-109">Ställ in EnableADAL = 0 så här:</span><span class="sxs-lookup"><span data-stu-id="1c5d1-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="1c5d1-110">Högerklicka på Start-knappen i Windows, välj **Kör,** skriv **regedit** och välj sedan **OK.**</span><span class="sxs-lookup"><span data-stu-id="1c5d1-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="1c5d1-111">Välj **Ja** om du vill tillåta registereditorn att göra ändringar på din enhet.</span><span class="sxs-lookup"><span data-stu-id="1c5d1-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="1c5d1-112">Lägg till ett DWORD-värde för **EnableADAL** i Registereditorn med inställningen **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="1c5d1-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="1c5d1-113">Mer information finns i Anslutningsproblem vid inloggning efter uppdatering till [Office 2016 version 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="1c5d1-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>