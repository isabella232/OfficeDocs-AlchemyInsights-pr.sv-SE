---
title: Licensproblem med Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148427"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="2a3c3-102">Licensproblem med Yammer</span><span class="sxs-lookup"><span data-stu-id="2a3c3-102">Yammer licensing issues</span></span>

<span data-ttu-id="2a3c3-103">Alla användare måste ha en licens för att använda Yammer Enterprise-tjänsten, men som standard kräver Yammer inte att användarna har licens att komma åt tjänsten.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="2a3c3-104">När en administratör ändrar inställningen för att blockera Microsoft 365-användare utan Yammer-licenser kan användare som inte har tilldelats en Yammer Enterprise-licens inte komma åt Yammer-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="2a3c3-105">Mer information finns [i Hantera Yammer-användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="2a3c3-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="2a3c3-106">När licenser tas bort från användare visas inte längre Yammer-panelen och andra tjänster kan använda licensborttagning för att dölja funktioner.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="2a3c3-107">I andra fall kan funktioner fortfarande visas men kräver licenstilldelning för att fungera.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="2a3c3-108">**Licensen uppdateras inte för användaren**</span><span class="sxs-lookup"><span data-stu-id="2a3c3-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="2a3c3-109">Ibland tilldelas en användare en licens men kan fortfarande inte komma åt Yammer.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="2a3c3-110">Det är mer sannolikt att fördröjningar uppstår när en masslicenstilldelning pågår.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="2a3c3-111">Yammer-användare kanske inte uppdateras i samma ordning som licenser ändras i Azure AD eftersom systemet körs asynkront.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="2a3c3-112">Vänta upp till 24 timmar innan du öppnar ett supportärende för att rapportera problem med licenssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="2a3c3-113">**Tilldelning av bulklicenser**</span><span class="sxs-lookup"><span data-stu-id="2a3c3-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="2a3c3-114">Licenser kan tilldelas via administrationscentret eller PowerShell-skript.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="2a3c3-115">Mer information finns i [Tilldela licenser till användare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) och Tilldela licenser till [användarkonton med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="2a3c3-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="2a3c3-116">Microsoft Support hjälper inte till att skapa skript, men dokumentation om Yammer-licenstilldelning är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="2a3c3-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="2a3c3-117">Mer information finns i [Hantera Yammer-licenser med Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="2a3c3-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>