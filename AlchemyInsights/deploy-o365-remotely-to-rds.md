---
title: Distribuera Office 365 ProPlus för delad användning på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959477"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="1360c-102">Distribuera Office 365 ProPlus för delad användning på RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="1360c-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="1360c-103">Så här distribuerar du Office 365 ProPlus med Remote Desktop Services (RDS), tidigare namngivna Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="1360c-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="1360c-104">Du måste ha en Microsoft 365 för affärsplan eller en Office 365-plan som innehåller Office 365 ProPlus, till exempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1360c-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="1360c-105">Office 365 Business och Office 365 Business Premium-abonnemang innehåller inte Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="1360c-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="1360c-106">Du måste aktivera [delad datoraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="1360c-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="1360c-107">Du kan också hämta och köra [Microsoft support och återställning assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Office 365 ProPlus i läget för delad datoraktivering.</span><span class="sxs-lookup"><span data-stu-id="1360c-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="1360c-108">Mer information om förutsättningar, installationsanvisningar och vägledning om anpassade installationer med hjälp av Office Deployment Tool finns i [distribuera office 365 ProPlus med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="1360c-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="1360c-109">Så här åtgärdar du fel som rör delad datoraktivering:</span><span class="sxs-lookup"><span data-stu-id="1360c-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="1360c-110">Se [Felsöka problem med aktivering av delade datorer för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="1360c-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="1360c-111">Se [återställa aktiveringstillståndet för Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="1360c-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="1360c-112">Om du vill installera Office 365 ProPlus på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, använder du följande steg:</span><span class="sxs-lookup"><span data-stu-id="1360c-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="1360c-113">Kontrollera vad Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="1360c-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="1360c-114">[Läs mer](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="1360c-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="1360c-115">Om det behövs växlar du till en annan Office 365-plan.</span><span class="sxs-lookup"><span data-stu-id="1360c-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="1360c-116">[Läs mer](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="1360c-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="1360c-117">Om Office redan är installerat på RDS-servern med andra Office 365-abonnemang avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="1360c-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="1360c-118">Till exempel, genom att gå till **Kontrollpanelen** > **Avinstallera ett program**.</span><span class="sxs-lookup"><span data-stu-id="1360c-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="1360c-119">Avinstallera med hjälp av [Microsoft support och Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du kör i problem.</span><span class="sxs-lookup"><span data-stu-id="1360c-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="1360c-120">På RDS-servern loggar du in på Microsoft 365 administratörscenter med ditt administratörskonto och [installerar Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="1360c-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="1360c-121">När Office har installerats ska ***du inte öppna eller logga in*** på några Office-program.</span><span class="sxs-lookup"><span data-stu-id="1360c-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="1360c-122">Aktivera delad datoraktivering genom att redigera registret på RDS-servern genom att följa dessa steg:</span><span class="sxs-lookup"><span data-stu-id="1360c-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="1360c-123">Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="1360c-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="1360c-124">Skriv **regedit**i rutan Öppna och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="1360c-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="1360c-125">Välj **Ja** när du tillfrågas om du vill tillåta att Registereditorn gör ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="1360c-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="1360c-126">I Registereditorn lägger du till ett strängvärde för **Sharedcomputerlicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \Software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="1360c-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="1360c-127">***Logga in som en slutanvändare*** på RDS-servern och [Kontrollera att aktivering av delade datorer är aktiverat för Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="1360c-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

