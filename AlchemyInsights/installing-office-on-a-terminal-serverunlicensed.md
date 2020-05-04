---
title: Installera kontor på en Terminal Server - Olicensierad
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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010632"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8a867-102">Installera Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="8a867-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8a867-103">För distribution av Microsoft 365-appar för företag på en Windows Server med fjärrskrivbordstjänster ( RDS), tidigare terminaltjänster:</span><span class="sxs-lookup"><span data-stu-id="8a867-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8a867-104">Du måste ha en Microsoft 365-prenumeration som innehåller Microsoft 365 Apps för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8a867-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8a867-105">Microsoft 365 Apps for business och Microsoft 365 Apps for business Premium-abonnemang innehåller inte Microsoft 365 Apps för företag.</span><span class="sxs-lookup"><span data-stu-id="8a867-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="8a867-106">Du måste aktivera [aktivering av delad dator](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8a867-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="8a867-107">Om du vill installera Microsoft 365 Apps for enterprise på RDS från Microsoft 365 admin center, ***som använder standardinstallationsinställningar,*** gör du så här.</span><span class="sxs-lookup"><span data-stu-id="8a867-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8a867-108">Du kan också hämta och köra [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365 Apps för företag i aktiveringsläge för delade datorer.</span><span class="sxs-lookup"><span data-stu-id="8a867-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8a867-109">Kontrollera vilken Microsoft 365-prenumeration du har.</span><span class="sxs-lookup"><span data-stu-id="8a867-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="8a867-110">Lära sig</span><span class="sxs-lookup"><span data-stu-id="8a867-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8a867-111">Om det behövs växlar du till en annan Microsoft 365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="8a867-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="8a867-112">Lära sig</span><span class="sxs-lookup"><span data-stu-id="8a867-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8a867-113">Om Office redan är installerat på RDS-servern med andra Microsoft 365-prenumerationer avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="8a867-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="8a867-114">Till exempel genom att \> gå till Kontrollpanelen Avinstallera ett program.</span><span class="sxs-lookup"><span data-stu-id="8a867-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8a867-115">Avinstallera med Hjälp av [Microsoft Support och Återställningsassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du har problem.</span><span class="sxs-lookup"><span data-stu-id="8a867-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8a867-116">Logga in på Microsoft 365-administrationscentret med administratörskontot på RDS-servern och [installera Microsoft 365 Apps för företag](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8a867-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8a867-117">När Office har ***installerats ska du inte öppna eller logga in på*** några Office-program.</span><span class="sxs-lookup"><span data-stu-id="8a867-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8a867-118">Aktivera delad datoraktivering på RDS-servern genom att redigera registret genom att följa dessa steg:</span><span class="sxs-lookup"><span data-stu-id="8a867-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8a867-119">Högerklicka på Windows-knappen i det nedre vänstra hörnet på skärmen och välj Kör.</span><span class="sxs-lookup"><span data-stu-id="8a867-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8a867-120">Skriv **regedit**i rutan Öppna och välj sedan OK.</span><span class="sxs-lookup"><span data-stu-id="8a867-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8a867-121">Välj Ja när du uppmanas att tillåta Registereditorn att göra ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="8a867-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8a867-122">Lägg till ett strängvärde för **SharedComputerLicensing** i Registereditorn med inställningen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8a867-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8a867-123">Logga in som ***slutanvändare på*** RDS-servern och [kontrollera att aktivering av delad dator är aktiverad för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8a867-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="8a867-124">Mer information om förutsättningar, installationsinstruktioner och vägledning om anpassade installationer med hjälp av Distributionsverktyget för Office finns i [Distribuera Microsoft 365-appar för företag med hjälp av Fjärrskrivbordstjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8a867-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="8a867-125">Information om hur du åtgärdar fel i samband med aktivering av delad dator finns [i Felsöka problem med aktivering av delad dator för Microsoft 365 Apps för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="8a867-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  