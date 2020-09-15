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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695305"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="f5992-102">Tom inloggnings skärm i Microsoft 365-appar</span><span class="sxs-lookup"><span data-stu-id="f5992-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="f5992-103">Lös problemet genom att pröva följande:</span><span class="sxs-lookup"><span data-stu-id="f5992-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="f5992-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="f5992-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="f5992-105">Återställ alternativen för Internet Explorer: gå **till**  >  **Internet alternativ**  >  **avancerade**  >  **Återställ inställningar för Internet Explorer** (Observera att du kommer att förlora anpassade inställningar) och försök sedan att logga in på Office igen.</span><span class="sxs-lookup"><span data-stu-id="f5992-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="f5992-106">Inaktivera Windows Defender Application Guard (WDAG) eller liknande brand vägg eller antivirus program:</span><span class="sxs-lookup"><span data-stu-id="f5992-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="f5992-107">Gå till **program**på kontroll panelen och välj **Aktivera eller inaktivera Windows-funktioner**.</span><span class="sxs-lookup"><span data-stu-id="f5992-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="f5992-108">Om Windows Defender Application Guard är aktiverat kan du försöka med att inaktivera det.</span><span class="sxs-lookup"><span data-stu-id="f5992-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="f5992-109">**Obs!** Du kan behöva starta om datorn.</span><span class="sxs-lookup"><span data-stu-id="f5992-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="f5992-110">Kontrol lera att plugin-programmet Microsoft. AAD. BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av något program eller brand vägg/antivirus program.</span><span class="sxs-lookup"><span data-stu-id="f5992-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="f5992-111">[Rensa Office-uppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Autentiseringshanteraren Manager.</span><span class="sxs-lookup"><span data-stu-id="f5992-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f5992-112">**Obs!** Register Sök vägarna för Office 2016 har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="f5992-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f5992-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f5992-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="f5992-114">Mer information finns i [anslutnings problem i Logga in efter uppdatering till Office 2016 version 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="f5992-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>