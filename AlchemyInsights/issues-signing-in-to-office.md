---
title: Problem att logga in på Office apps
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938359"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="9c653-102">Tom inloggningsskärmen i Office apps</span><span class="sxs-lookup"><span data-stu-id="9c653-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="9c653-103">Om du vill åtgärda det här problemet kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="9c653-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9c653-104">Installera de senaste uppdateringarna för [Windows](https://support.microsoft.com/help/4027667/windows-10-update) och [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9c653-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9c653-105">Återställ Internet Explorer-alternativ: Gå till **Verktyg** > **Internet-alternativ** > **Avancerat** > **Återställ inställningar för Internet Explorer** (Observera att du kommer att förlora anpassade inställningar) och försök sedan logga in på Office igen.</span><span class="sxs-lookup"><span data-stu-id="9c653-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9c653-106">Inaktivera Windows Defender programmet Guard (WDAG) eller något liknande brandvägg eller anti-virus program:</span><span class="sxs-lookup"><span data-stu-id="9c653-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9c653-107">Gå till **program**på Kontrollpanelen och klicka på **Aktivera Windows-funktioner på eller av**.</span><span class="sxs-lookup"><span data-stu-id="9c653-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9c653-108">Om Windows Defender programmet Guard är aktiverad kan du prova att inaktivera den.</span><span class="sxs-lookup"><span data-stu-id="9c653-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9c653-109">**Observera:** Du kan behöva starta om datorn.</span><span class="sxs-lookup"><span data-stu-id="9c653-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9c653-110">Se till att Microsoft.AAD.BrokerPlugin [Ledsagardokumentet WAM plugin-program](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) inte blockeras av ett program eller en brandvägg/mot-virus program.</span><span class="sxs-lookup"><span data-stu-id="9c653-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9c653-111">[Rensa Office autentiseringsuppgifter](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) med hjälp av Windows Referenshanteraren.</span><span class="sxs-lookup"><span data-stu-id="9c653-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9c653-112">**Observera:** Registersökvägar 2016 för Office har ändrats till 16,0.</span><span class="sxs-lookup"><span data-stu-id="9c653-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9c653-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9c653-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9c653-114">Mer information finns i [anslutning problem i logga in efter uppdatering till Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9c653-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>