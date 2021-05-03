---
title: Distribuera tillägg för Microsoft 365 program
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125687"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="1938e-102">Distribuera tillägg för Microsoft 365 program</span><span class="sxs-lookup"><span data-stu-id="1938e-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="1938e-103">Centraliserad distribution är det rekommenderade sättet Office distribuera tillägg till användare och grupper inom organisationen.</span><span class="sxs-lookup"><span data-stu-id="1938e-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="1938e-104">Följ stegen nedan för att distribuera tillägg:</span><span class="sxs-lookup"><span data-stu-id="1938e-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="1938e-105">**Obs!** Information om hur du installerar tillägg Office enskilda användare finns i Visa, hantera och installera tillägg [i Office program.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="1938e-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="1938e-106">Se också till att enskilda Office Store-tillägg är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="1938e-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="1938e-107">Kontrollera att miljön uppfyller kraven för distribution av tillägg med hjälp av centraliserad distribution.</span><span class="sxs-lookup"><span data-stu-id="1938e-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="1938e-108">Mer information finns i [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="1938e-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="1938e-109">Gå **Inställningar**  >  **appar Skaffa**  >  **appar** i administrationscentret Microsoft 365 och distribuera tillägg.</span><span class="sxs-lookup"><span data-stu-id="1938e-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="1938e-110">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="1938e-110">Notes:</span></span> 

- <span data-ttu-id="1938e-111">Integrerade appar kräver att administratören har global administratör Exchange administratörsbehörighet.</span><span class="sxs-lookup"><span data-stu-id="1938e-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="1938e-112">När du distribuerar tillägg till flera användare rekommenderar vi att du gör tilldelningar genom att använda grupper istället för enskilda användare.</span><span class="sxs-lookup"><span data-stu-id="1938e-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="1938e-113">Mer information finns i [Att tänka på när du tilldelar ett tillägg till användare och grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="1938e-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="1938e-114">Centraliserad distribution stöder inte användare i kapslade grupper eller grupper som har överordnade grupper.</span><span class="sxs-lookup"><span data-stu-id="1938e-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="1938e-115">Mer information finns i [Användar- och gruppuppgifter.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="1938e-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="1938e-116">Kontrollera att Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') har aktiverats för användarna att logga in.</span><span class="sxs-lookup"><span data-stu-id="1938e-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="1938e-117">Mer information finns i [Konfigurera appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="1938e-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="1938e-118">Om du får problem med att distribuera tillägg med hjälp av integrerade appar kan du prova att [distribuera med hjälp av tillägg.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="1938e-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="1938e-119">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="1938e-119">For more information, see:</span></span>

<span data-ttu-id="1938e-120">[Distribuera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Hantera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Använda PowerShell-cmdlets för](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) centraliserad distribution för att hantera tillägg 
 [Publicera Office tillägg med hjälp av centraliserad distribution via Microsoft 365 administrationscenter](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Felsökning: Användaren ser inte tillägg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Felsöka användarfel med Office tillägg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="1938e-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>