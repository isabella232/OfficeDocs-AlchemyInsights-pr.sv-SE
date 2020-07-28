---
title: Styra automatiska uppdateringar för Office Apps
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
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439926"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="03832-102">Styra automatiska uppdateringar för Office Apps</span><span class="sxs-lookup"><span data-stu-id="03832-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="03832-103">Som standard hämtas uppdateringar för Office Apps automatiskt och tillämpas i bakgrunden utan att användaren behöver göra något.</span><span class="sxs-lookup"><span data-stu-id="03832-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="03832-104">Administratörer kan dock styra hur uppdateringar tillämpas med hjälp av Office Update-inställningar.</span><span class="sxs-lookup"><span data-stu-id="03832-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="03832-105">Med uppdateringsinställningarna kan administratörer aktivera eller inaktivera automatiska uppdateringar, visa eller dölja knappen **Uppdatera nu** i Office, ange tidsgränser för uppdateringar med mera.</span><span class="sxs-lookup"><span data-stu-id="03832-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="03832-106">Detaljerad information finns i:</span><span class="sxs-lookup"><span data-stu-id="03832-106">For detailed information, see:</span></span>

- [<span data-ttu-id="03832-107">Konfigurera uppdateringsinställningar för Office</span><span class="sxs-lookup"><span data-stu-id="03832-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="03832-108">Automatisk uppdatering för Office är inte aktiverat</span><span class="sxs-lookup"><span data-stu-id="03832-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="03832-109">Definiera hur Office uppdateras när det har installerats</span><span class="sxs-lookup"><span data-stu-id="03832-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="03832-110">Så här granskar du de befintliga uppdateringsinställningarna som tillämpas på en klientdator:</span><span class="sxs-lookup"><span data-stu-id="03832-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="03832-111">Öppna Registereditorn genom att gå till **Starta**  >  **Kör**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="03832-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="03832-112">Växla till följande plats och granska inställningarna för Office Update:</span><span class="sxs-lookup"><span data-stu-id="03832-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="03832-113">a.</span><span class="sxs-lookup"><span data-stu-id="03832-113">a.</span></span> <span data-ttu-id="03832-114">HKEY_LOCAL_MACHINE\PROGRAMVARA\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="03832-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="03832-115">b.</span><span class="sxs-lookup"><span data-stu-id="03832-115">b.</span></span> <span data-ttu-id="03832-116">Klicka på Tillrun\Konfiguration</span><span class="sxs-lookup"><span data-stu-id="03832-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="03832-117">**Anm.)**  Om OfficeMgmtCOM-nyckeln är inställd kan meddelandet "Uppdateringar hanteras av **Office**systemadministratören" visas i  >  **Account**  >  **Office-uppdateringar**för Office-konto .</span><span class="sxs-lookup"><span data-stu-id="03832-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="03832-118">Mer information finns i [Hantera uppdateringar av Microsoft 365-appar med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="03832-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  