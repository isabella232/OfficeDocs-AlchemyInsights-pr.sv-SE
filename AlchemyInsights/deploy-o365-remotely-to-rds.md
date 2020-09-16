---
title: Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745553"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="d0709-102">Distribuera Microsoft 365-appar för företag för delad användning på RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="d0709-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="d0709-103">Så här distribuerar du Microsoft 365-appar för företag med fjärr skrivbords tjänster (RDS), tidigare namngivna Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="d0709-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="d0709-104">Du måste ha ett Microsoft 365 för företag-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d0709-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="d0709-105">Microsoft 365-apparna för företag och Microsoft 365 Business Premium standard-abonnemang inkluderar inte Microsoft 365-appar för företag.</span><span class="sxs-lookup"><span data-stu-id="d0709-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="d0709-106">Du måste aktivera [delad dator aktivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d0709-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="d0709-107">Du kan också ladda ned och köra [Microsoft-assistenten för support och återställning](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365-appar för företag i aktiverings läget för delad dator.</span><span class="sxs-lookup"><span data-stu-id="d0709-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="d0709-108">Mer information om förutsättningar, konfigurations instruktioner och vägledning om anpassade installationer med hjälp av distributions verktyget för Office finns i [distribuera Microsoft 365-appar för företag med hjälp av fjärr skrivbords tjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d0709-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="d0709-109">Så här löser du problem med att aktivera en delad dator:</span><span class="sxs-lookup"><span data-stu-id="d0709-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="d0709-110">Se [Felsöka problem med att aktivera delad dator för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d0709-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="d0709-111">Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="d0709-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="d0709-112">Om du vill installera Microsoft 365-appar för företag på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, gör du så här:</span><span class="sxs-lookup"><span data-stu-id="d0709-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="d0709-113">Kontrol lera vilken prenumeration du har.</span><span class="sxs-lookup"><span data-stu-id="d0709-113">Check what subscription you have.</span></span> <span data-ttu-id="d0709-114">[Läs mer](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="d0709-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="d0709-115">Byt eventuellt till ett annat abonnemang.</span><span class="sxs-lookup"><span data-stu-id="d0709-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="d0709-116">[Läs mer](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="d0709-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="d0709-117">Om Office redan är installerat på RDS-servern med andra Microsoft-abonnemang avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="d0709-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="d0709-118">Till exempel genom att gå till **kontroll panelen**  >  **Avinstallera ett program**.</span><span class="sxs-lookup"><span data-stu-id="d0709-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="d0709-119">Avinstallera med [Microsoft support-och återställnings assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du stöter på problem.</span><span class="sxs-lookup"><span data-stu-id="d0709-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="d0709-120">Logga in på administrations centret för Microsoft 365 med ditt administratörs konto och [Installera Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d0709-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="d0709-121">När Office är installerat kan du ***inte öppna eller logga*** in på något Office-program.</span><span class="sxs-lookup"><span data-stu-id="d0709-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="d0709-122">Aktivera delad dator aktivering på RDS-servern genom att redigera registret genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="d0709-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="d0709-123">Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="d0709-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="d0709-124">I rutan Öppna skriver du **regedit**och väljer sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0709-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="d0709-125">Välj **Ja** när du uppmanas att tillåta att Registereditorn gör ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="d0709-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="d0709-126">I Registereditorn lägger du till ett sträng värde för **SharedComputerLicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d0709-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="d0709-127">***Logga in som slutanvändare*** på RDS-servern och [kontrol lera att aktivera delad dator är aktiverat för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d0709-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

