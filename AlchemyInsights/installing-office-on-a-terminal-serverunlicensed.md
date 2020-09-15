---
title: Installera Office på en terminalserver-olicensierad
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663135"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f5856-102">Installera Office på en terminalserver</span><span class="sxs-lookup"><span data-stu-id="f5856-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f5856-103">För distribution av Microsoft 365-appar för företag på en Windows Server med fjärr skrivbords tjänster (RDS), tidigare kallat Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="f5856-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f5856-104">Du måste ha en Microsoft 365-prenumeration som innehåller Microsoft 365-appar för företag, till exempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f5856-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="f5856-105">Microsoft 365-apparna för företag och Microsoft 365-appar för företag Premium-program inkluderar inte Microsoft 365-appar för företag.</span><span class="sxs-lookup"><span data-stu-id="f5856-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="f5856-106">Du måste aktivera [delad dator aktivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="f5856-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="f5856-107">Om du vill installera Microsoft 365-appar för företag på RDS från Microsoft 365 Admin Center, ***som använder standardinställningarna för installation***, gör du följande:</span><span class="sxs-lookup"><span data-stu-id="f5856-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="f5856-108">Du kan också ladda ned och köra [Microsoft-assistenten för support och återställning](https://aka.ms/SaRA_OfficeSCA_M365Portal) för att installera Microsoft 365-appar för företag i aktiverings läget för delad dator.</span><span class="sxs-lookup"><span data-stu-id="f5856-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="f5856-109">Kolla vilken Microsoft 365-prenumeration du har.</span><span class="sxs-lookup"><span data-stu-id="f5856-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="f5856-110">Lär dig hur</span><span class="sxs-lookup"><span data-stu-id="f5856-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="f5856-111">Om det behövs byter du till en annan Microsoft 365-prenumeration.</span><span class="sxs-lookup"><span data-stu-id="f5856-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="f5856-112">Lär dig hur</span><span class="sxs-lookup"><span data-stu-id="f5856-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="f5856-113">Om Office redan är installerat på RDS-servern med andra Microsoft 365-abonnemang avinstallerar du det.</span><span class="sxs-lookup"><span data-stu-id="f5856-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="f5856-114">Till exempel genom att gå till kontroll panelen \> Avinstallera ett program.</span><span class="sxs-lookup"><span data-stu-id="f5856-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="f5856-115">Avinstallera med [Microsoft support-och återställnings assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) om du stöter på problem.</span><span class="sxs-lookup"><span data-stu-id="f5856-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="f5856-116">Logga in på administrations centret för Microsoft 365 med ditt administratörs konto och [Installera Microsoft 365-appar för företag](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="f5856-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="f5856-117">När Office är installerat kan du ***inte öppna eller logga*** in på något Office-program.</span><span class="sxs-lookup"><span data-stu-id="f5856-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="f5856-118">Aktivera delad dator aktivering på RDS-servern genom att redigera registret genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="f5856-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="f5856-119">Högerklicka på Windows-knappen i det nedre vänstra hörnet av skärmen och välj Kör.</span><span class="sxs-lookup"><span data-stu-id="f5856-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="f5856-120">I rutan Öppna skriver du **regedit**och väljer sedan OK.</span><span class="sxs-lookup"><span data-stu-id="f5856-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="f5856-121">Välj Ja när du uppmanas att tillåta att Registereditorn gör ändringar på enheten.</span><span class="sxs-lookup"><span data-stu-id="f5856-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="f5856-122">I Registereditorn lägger du till ett sträng värde för **SharedComputerLicensing** med en inställning på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="f5856-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="f5856-123">***Logga in som slutanvändare*** på RDS-servern och [kontrol lera att aktivera delad dator är aktiverat för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="f5856-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="f5856-124">Mer information om förutsättningar, installations anvisningar och vägledning om anpassade installationer med hjälp av distributions verktyget för Office finns i [distribuera Microsoft 365-appar för företag med hjälp av fjärr skrivbords tjänster](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="f5856-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="f5856-125">Information om hur du åtgärdar problem med att aktivera en delad dator finns i [Felsöka problem med delad dator aktivering för Microsoft 365-appar för företag](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="f5856-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  