---
title: Installera Office på en terminalserver-olicensierad
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205427"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="91be3-102">Installera Office på en terminalserver</span><span class="sxs-lookup"><span data-stu-id="91be3-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="91be3-103">För distribution av Office 365 ProPlus på en Windows-Server med hjälp av Remote Desktop Services (RDS), tidigare namngivna Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="91be3-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="91be3-104">Du måste ha en Office 365-plan som innehåller Office 365 ProPlus, till exempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="91be3-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="91be3-105">Office 365 Business och Office 365 Business Premium-abonnemang innehåller inte Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="91be3-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="91be3-106">Du måste aktivera [delad datoraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="91be3-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="91be3-107">Om du vill installera Office 365 ProPlus på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, använder du följande steg.</span><span class="sxs-lookup"><span data-stu-id="91be3-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="91be3-108">Du kan också hämta och köra [Microsoft support och återställning assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Office 365 ProPlus i läget för delad datoraktivering.</span><span class="sxs-lookup"><span data-stu-id="91be3-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="91be3-109">Kontrollera vad Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="91be3-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="91be3-110">Lära sig</span><span class="sxs-lookup"><span data-stu-id="91be3-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="91be3-111">Om det behövs växlar du till en annan Office 365-plan.</span><span class="sxs-lookup"><span data-stu-id="91be3-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="91be3-112">Lära sig</span><span class="sxs-lookup"><span data-stu-id="91be3-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="91be3-113">Om Office redan är installerat på RDS-servern med andra Office 365-abonnemang avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="91be3-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="91be3-114">Till exempel, genom att gå till kontroll \> panelen Avinstallera ett program.</span><span class="sxs-lookup"><span data-stu-id="91be3-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="91be3-115">Avinstallera med hjälp av [Microsoft support och Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du kör i problem.</span><span class="sxs-lookup"><span data-stu-id="91be3-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="91be3-116">På RDS-servern loggar du in på Microsoft 365 administratörscenter med ditt administratörskonto och [installerar Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="91be3-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="91be3-117">När Office har installerats ska ***du inte öppna eller logga in*** på några Office-program.</span><span class="sxs-lookup"><span data-stu-id="91be3-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="91be3-118">Aktivera delad datoraktivering genom att redigera registret på RDS-servern genom att följa dessa steg:</span><span class="sxs-lookup"><span data-stu-id="91be3-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="91be3-119">Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj Kör.</span><span class="sxs-lookup"><span data-stu-id="91be3-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="91be3-120">Skriv **regedit**i rutan Öppna och välj sedan OK.</span><span class="sxs-lookup"><span data-stu-id="91be3-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="91be3-121">Välj Ja när du tillfrågas om du vill tillåta att Registereditorn gör ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="91be3-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="91be3-122">I Registereditorn lägger du till ett strängvärde för **Sharedcomputerlicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="91be3-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="91be3-123">***Logga in som en slutanvändare*** på RDS-servern och [Kontrollera att aktivering av delade datorer är aktiverat för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="91be3-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="91be3-124">Mer information om förutsättningar, installationsanvisningar och vägledning om anpassade installationer med hjälp av Office Deployment Tool finns i [distribuera office 365 ProPlus med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="91be3-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="91be3-125">Om du vill åtgärda fel i samband med aktivering av delade datorer läser du [Felsöka problem med aktivering av delade datorer för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="91be3-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  