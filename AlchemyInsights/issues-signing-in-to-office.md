---
title: Problem med att logga in på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579919"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6857b-102">Tom inloggningsskärm i Microsoft 365-appar</span><span class="sxs-lookup"><span data-stu-id="6857b-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6857b-103">Försök med följande om du vill åtgärda problemet:</span><span class="sxs-lookup"><span data-stu-id="6857b-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6857b-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6857b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6857b-105">Återställ Internet Explorer-alternativ: Gå till **Verktyg**  >  **Internet-alternativ**  >  **Avancerade**  >  **återställningsinställningar för Internet Explorer** (observera att du kommer att förlora anpassade inställningar) och försök sedan logga in på Office igen.</span><span class="sxs-lookup"><span data-stu-id="6857b-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6857b-106">Inaktivera Windows Defender Application Guard (WDAG) eller liknande brandväggs- eller antivirusprogram:</span><span class="sxs-lookup"><span data-stu-id="6857b-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6857b-107">Gå till Program **på**Kontrollpanelen och välj sedan **Aktivera eller inaktivera Windows-funktioner.**</span><span class="sxs-lookup"><span data-stu-id="6857b-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6857b-108">Om Windows Defender Application Guard är aktiverat kan du prova att inaktivera den.</span><span class="sxs-lookup"><span data-stu-id="6857b-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6857b-109">**Anm.:** Du kan behöva starta om datorn.</span><span class="sxs-lookup"><span data-stu-id="6857b-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6857b-110">Kontrollera att plugin-programmet Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av något program eller ett antivirusprogram för brandväggar/antivirusprogram.</span><span class="sxs-lookup"><span data-stu-id="6857b-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6857b-111">[Rensa Office-autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med Windows-autentiseringshanteraren.</span><span class="sxs-lookup"><span data-stu-id="6857b-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6857b-112">**Anm.:** Registersökvägarna för Office 2016 har ändrats till 16.0.</span><span class="sxs-lookup"><span data-stu-id="6857b-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6857b-113">(T.ex. \Programvara\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6857b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6857b-114">Mer information finns [i Anslutningsproblem i inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6857b-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>