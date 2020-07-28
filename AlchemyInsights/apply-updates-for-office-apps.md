---
title: Installera uppdateringar för Office-appar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: b5952feaac7ac51faed2a3399c68a87a4227b165
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440153"
---
# <a name="apply-updates-for-office-apps"></a><span data-ttu-id="5e659-102">Installera uppdateringar för Office-appar</span><span class="sxs-lookup"><span data-stu-id="5e659-102">Apply updates for Office apps</span></span>

<span data-ttu-id="5e659-103">Som standard är uppdateringar för Office Apps kostnadsfria, hämtade automatiskt och tillämpas i bakgrunden utan att användaren behöver göra något.</span><span class="sxs-lookup"><span data-stu-id="5e659-103">By default, updates for Office Apps are free, downloaded automatically, and applied in the background without any user intervention.</span></span> <span data-ttu-id="5e659-104">Om du vill köra uppdateringar manuellt om du stöter på problem med att installera uppdateringar läser du [Installera Office-uppdateringar](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="5e659-104">To run updates manually if you are running into issues applying updates, see [Install Office updates](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span> <span data-ttu-id="5e659-105">Mer information finns i [Felsöka installation av Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).</span><span class="sxs-lookup"><span data-stu-id="5e659-105">For more information, see [Troubleshoot installing Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).</span></span>

<span data-ttu-id="5e659-106">Om du vill hantera Office-uppdateringar för användarna bör du tänka på följande:</span><span class="sxs-lookup"><span data-stu-id="5e659-106">To manage Office updates for your users, consider these options:</span></span>

- <span data-ttu-id="5e659-107">Välj rätt Office Update Channel för din organisation baserat på önskad frekvens av uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="5e659-107">Choose the right Office Update Channel for your organization based on the desired frequency of updates.</span></span> <span data-ttu-id="5e659-108">Mer information finns i [Översikt över uppdateringskanaler för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5e659-108">To learn how, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).</span></span>

- <span data-ttu-id="5e659-109">Bestäm om du vill installera uppdateringar automatiskt från internet eller från en lokal resurs.</span><span class="sxs-lookup"><span data-stu-id="5e659-109">Decide whether to apply updates automatically from the internet or from an on-premises share.</span></span> <span data-ttu-id="5e659-110">Mer information finns i [Välja hur du hanterar uppdateringar av Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5e659-110">To learn how, see [Choose how to manage updates to Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).</span></span>

- <span data-ttu-id="5e659-111">Granska Office Update-inställningar för att styra hur uppdateringar tillämpas på slutanvändarens datorer:</span><span class="sxs-lookup"><span data-stu-id="5e659-111">Review Office Update Settings to control how updates are applied to end user machines:</span></span>

    - <span data-ttu-id="5e659-112">[Konfigurera uppdateringsinställningar för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5e659-112">[Configure update settings for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).</span></span>
    - <span data-ttu-id="5e659-113">[Definiera hur Office uppdateras när det har installerats](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).</span><span class="sxs-lookup"><span data-stu-id="5e659-113">[Define how Office is updated after it's installed](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).</span></span>

<span data-ttu-id="5e659-114">När du distribuerar Office-appar till flera användare använder du verktyget Anpassning av Office för att skapa konfigurationsfiler för distribution och konfigurera Office-uppdateringar med hjälp av Office-distributionsverktyget.</span><span class="sxs-lookup"><span data-stu-id="5e659-114">When deploying Office apps to multiple users, use the Office Customization tool to build configuration files for deployment, and configure Office updates by using the Office Deployment tool.</span></span> <span data-ttu-id="5e659-115">Mer information finns [i Översikt över Anpassningsverktyget för Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) och [office-distributionsverktyget](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5e659-115">For more info, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) and the [Office Deployment tool](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

- <span data-ttu-id="5e659-116">Ett exempel på hur du konfigurerar användargrupper för att distribuera Office-uppdateringar finns i [Distribuera Microsoft 365-appar från en lokal källa](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).</span><span class="sxs-lookup"><span data-stu-id="5e659-116">For an example of how to setup user groups to deploy Office updates, see [Deploy Microsoft 365 Apps from a local source](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).</span></span>
-   <span data-ttu-id="5e659-117">Överväg att använda ForceAppShutdown-inställningen om Office-uppdateringar inte tillämpas på några användare på grund av öppna Office-appar.</span><span class="sxs-lookup"><span data-stu-id="5e659-117">Consider using the ForceAppShutdown setting in case Office updates are not getting applied to a few users because of open Office apps.</span></span> <span data-ttu-id="5e659-118">Mer information finns i [egenskapen FORCEAPPSHUTDOWN (en del av egenskapselementet).](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)</span><span class="sxs-lookup"><span data-stu-id="5e659-118">For more info, see the [FORCEAPPSHUTDOWN property (part of Property element)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element).</span></span> 

<span data-ttu-id="5e659-119">**Se även**</span><span class="sxs-lookup"><span data-stu-id="5e659-119">**See also**</span></span>

<span data-ttu-id="5e659-120">[Översikt över uppdateringsprocessen för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5e659-120">[Overview of the update process for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).</span></span>  
<span data-ttu-id="5e659-121">[Släpp information för uppdateringar till Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).</span><span class="sxs-lookup"><span data-stu-id="5e659-121">[Release information for updates to Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).</span></span>  
<span data-ttu-id="5e659-122">[Hantera uppdateringar av Microsoft 365-appar med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="5e659-122">[Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).</span></span>  
