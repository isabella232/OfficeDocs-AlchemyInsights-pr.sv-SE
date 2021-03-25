---
title: Distribuera Microsoft 365-program för företag för delad användning i RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200691"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="9575e-102">Distribuera Microsoft 365-program för företag för delad användning i RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="9575e-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="9575e-103">Så här distribuerar du Microsoft 365-appar för företag med Fjärrskrivbordstjänster (RDS) som tidigare hette Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="9575e-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="9575e-104">Du måste ha ett Microsoft 365 för företag-abonnemang eller ett Office 365-abonnemang som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise, E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="9575e-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="9575e-105">Microsoft 365-programmen för företag och Microsoft 365 Business Standard-abonnemangen innehåller inte Microsoft 365-appar för företag.</span><span class="sxs-lookup"><span data-stu-id="9575e-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="9575e-106">Du måste aktivera [aktivering på delad dator.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="9575e-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="9575e-107">Du kan också ladda ned och köra [Microsoft Support- och](https://aka.ms/SaRA_OfficeSCA_M365Portal) återställningsassistenten för att installera Microsoft 365-appar för företag i läget för aktivering på delad dator.</span><span class="sxs-lookup"><span data-stu-id="9575e-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="9575e-108">Mer information om krav, installationsanvisningar och vägledning för anpassade installationer med hjälp av distributionsverktyget för Office finns i Distribuera [Microsoft 365-program](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)för företag med hjälp av Fjärrskrivbordstjänster.</span><span class="sxs-lookup"><span data-stu-id="9575e-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="9575e-109">Så här åtgärdar du fel som rör aktivering av delad dator:</span><span class="sxs-lookup"><span data-stu-id="9575e-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="9575e-110">Se [Felsöka problem med aktivering av delad dator för Microsoft 365-program för företag.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="9575e-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="9575e-111">Se [Återställa Microsoft 365-appar för företagsaktiveringsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="9575e-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="9575e-112">Om du vill installera Microsoft 365-appar för företag på RDS från administrationscentret för Microsoft 365 ***med*** standardinstallationsinställningarna gör du så här:</span><span class="sxs-lookup"><span data-stu-id="9575e-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="9575e-113">Kontrollera vilken prenumeration du har.</span><span class="sxs-lookup"><span data-stu-id="9575e-113">Check what subscription you have.</span></span> <span data-ttu-id="9575e-114">[Läs mer](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="9575e-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="9575e-115">Byt till en annan prenumeration om det behövs.</span><span class="sxs-lookup"><span data-stu-id="9575e-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="9575e-116">[Läs mer](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="9575e-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="9575e-117">Om Office redan är installerat på RDS-servern med några andra Microsoft-prenumerationer avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="9575e-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="9575e-118">Genom att till exempel gå till **Kontrollpanelen Avinstallera**  >  **ett program**.</span><span class="sxs-lookup"><span data-stu-id="9575e-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="9575e-119">Avinstallera med [Microsoft Support- och återställningsassistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du har problem.</span><span class="sxs-lookup"><span data-stu-id="9575e-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="9575e-120">På RDS-servern loggar du in på administrationscentret för Microsoft 365 med ditt administratörskonto och installerar [Microsoft 365-program för företag.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="9575e-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="9575e-121">När Office har installerats ***ska du inte öppna eller logga in i*** något Office-program.</span><span class="sxs-lookup"><span data-stu-id="9575e-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="9575e-122">Aktivera aktivering av delad dator på RDS-servern genom att redigera registret så här:</span><span class="sxs-lookup"><span data-stu-id="9575e-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="9575e-123">Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj **Kör**.</span><span class="sxs-lookup"><span data-stu-id="9575e-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="9575e-124">Skriv regedit i rutan **Öppna** klicka sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="9575e-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="9575e-125">Välj **Ja** när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="9575e-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="9575e-126">I Registereditorn lägger du till strängvärdet **SharedComputerLicensing** med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="9575e-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="9575e-127">Logga ***in*** som slutanvändare på RDS-servern och kontrollera att aktivering av delade datorer är aktiverat för [Microsoft 365-appar för företag.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="9575e-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
