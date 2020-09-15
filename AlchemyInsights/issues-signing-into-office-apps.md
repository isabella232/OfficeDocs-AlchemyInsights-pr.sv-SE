---
title: Problem med att logga in i Microsoft 365-appar
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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695197"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="3bba9-102">Att åtgärda Microsoft 365-apparna "din dators betrodda plattformsmodulen fungerar inte korrekt"</span><span class="sxs-lookup"><span data-stu-id="3bba9-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="3bba9-103">Lös problemet genom att prova med följande:</span><span class="sxs-lookup"><span data-stu-id="3bba9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3bba9-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="3bba9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="3bba9-105">[Rensa Office-uppgifter](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.</span><span class="sxs-lookup"><span data-stu-id="3bba9-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3bba9-106">**Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="3bba9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3bba9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3bba9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3bba9-108">Pröva [användar återställnings processen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) för att åtgärda fel i TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="3bba9-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="3bba9-109">Ange EnableADAL = 0 så här:</span><span class="sxs-lookup"><span data-stu-id="3bba9-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="3bba9-110">Högerklicka på Start-knappen i Windows, Välj **Kör**, Skriv **regedit**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="3bba9-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="3bba9-111">Välj **Ja** om du vill tillåta att Registereditorn gör ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="3bba9-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="3bba9-112">I Registereditorn lägger du till ett DWORD-värde för **EnableADAL** med en inställning på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="3bba9-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="3bba9-113">Mer information finns i [anslutnings problem i Logga in efter uppdatering till Office 2016 version 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="3bba9-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>