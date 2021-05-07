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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233552"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="48c9d-102">Distribuera tillägg för Microsoft 365 program</span><span class="sxs-lookup"><span data-stu-id="48c9d-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="48c9d-103">Centraliserad distribution är det rekommenderade sättet Office distribuera tillägg till användare och grupper inom organisationen.</span><span class="sxs-lookup"><span data-stu-id="48c9d-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="48c9d-104">Följ stegen nedan för att distribuera tillägg:</span><span class="sxs-lookup"><span data-stu-id="48c9d-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="48c9d-105">**Obs!** Information om hur du installerar tillägg Office enskilda användare finns i Visa, hantera och installera tillägg [i Office program.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="48c9d-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="48c9d-106">Se också till att enskilda Office Store-tillägg är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="48c9d-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="48c9d-107">Mer information finns i Förhindra att tillägg hämtas genom att stänga av Office Store för alla klienter [(utom Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span><span class="sxs-lookup"><span data-stu-id="48c9d-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="48c9d-108">Kontrollera att miljön uppfyller kraven för distribution av tillägg med hjälp av centraliserad distribution.</span><span class="sxs-lookup"><span data-stu-id="48c9d-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="48c9d-109">Mer information finns i [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="48c9d-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="48c9d-110">Gå **Inställningar**  >  **appar Skaffa**  >  **appar** i administrationscentret Microsoft 365 och distribuera tillägg.</span><span class="sxs-lookup"><span data-stu-id="48c9d-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="48c9d-111">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="48c9d-111">Notes:</span></span> 

- <span data-ttu-id="48c9d-112">Integrerade appar kräver att administratören har global administratör Exchange administratörsbehörighet.</span><span class="sxs-lookup"><span data-stu-id="48c9d-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="48c9d-113">När du distribuerar tillägg till flera användare rekommenderar vi att du gör tilldelningar genom att använda grupper istället för enskilda användare.</span><span class="sxs-lookup"><span data-stu-id="48c9d-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="48c9d-114">Mer information finns i [Att tänka på när du tilldelar ett tillägg till användare och grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="48c9d-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="48c9d-115">Centraliserad distribution stöder inte användare i kapslade grupper eller grupper som har överordnade grupper.</span><span class="sxs-lookup"><span data-stu-id="48c9d-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="48c9d-116">Mer information finns i [Användar- och gruppuppgifter.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="48c9d-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="48c9d-117">Kontrollera att Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') har aktiverats för användarna att logga in.</span><span class="sxs-lookup"><span data-stu-id="48c9d-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="48c9d-118">Mer information finns i [Konfigurera appegenskaper](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="48c9d-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="48c9d-119">Om du får problem med att distribuera tillägg med hjälp av integrerade appar kan du prova att [distribuera med hjälp av tillägg.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="48c9d-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="48c9d-120">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="48c9d-120">For more information, see:</span></span>

<span data-ttu-id="48c9d-121">[Distribuera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Hantera tillägg i administrationscentret](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Använda PowerShell-cmdlets för](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) centraliserad distribution för att hantera tillägg 
 [Publicera Office tillägg med hjälp av centraliserad distribution via Microsoft 365 administrationscenter](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Felsökning: Användaren ser inte tillägg](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Felsöka användarfel med Office tillägg](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="48c9d-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>