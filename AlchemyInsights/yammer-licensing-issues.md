---
title: Problem med Yammer-licenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657294"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="02426-102">Problem med Yammer-licenser</span><span class="sxs-lookup"><span data-stu-id="02426-102">Yammer licensing issues</span></span>

<span data-ttu-id="02426-103">Alla användare måste ha en licens för att använda Yammer Enterprise-tjänsten, men som standard är Yammer inte att användare har en licens för att få åtkomst till tjänsten.</span><span class="sxs-lookup"><span data-stu-id="02426-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="02426-104">När en administratör ändrar inställningen för att blockera Microsoft 365-användare utan Yammer-licenser, får inte användare som inte har tilldelats Yammer-licenser åtkomst till Yammer-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="02426-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="02426-105">Mer information finns i [hantera användar licenser för Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="02426-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="02426-106">När licenser tas bort från användarna visas inte Yammer-panelen längre och andra tjänster kan använda licens borttagning för att dölja funktioner.</span><span class="sxs-lookup"><span data-stu-id="02426-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="02426-107">I andra fall kan funktioner fortfarande visas men kräver tilldelning av licenser.</span><span class="sxs-lookup"><span data-stu-id="02426-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="02426-108">**Licensen uppdateras inte för användaren**</span><span class="sxs-lookup"><span data-stu-id="02426-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="02426-109">Ibland tilldelas en användare en licens men kan fortfarande inte komma åt Yammer.</span><span class="sxs-lookup"><span data-stu-id="02426-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="02426-110">Det är ofta större att det uppstår fördröjningar när en Mass licens tilldelning pågår.</span><span class="sxs-lookup"><span data-stu-id="02426-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="02426-111">Yammer-användare kanske inte uppdateras i samma ordning som licenser ändras i Azure AD eftersom systemet körs asynkront.</span><span class="sxs-lookup"><span data-stu-id="02426-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="02426-112">Vänta 24 timmar innan du öppnar ett support ärende för att rapportera synkroniseringsproblem.</span><span class="sxs-lookup"><span data-stu-id="02426-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="02426-113">**Tilldelning av Mass licenser**</span><span class="sxs-lookup"><span data-stu-id="02426-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="02426-114">Licenser kan tilldelas via administrations centret eller PowerShell-skript.</span><span class="sxs-lookup"><span data-stu-id="02426-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="02426-115">Mer information finns i [tilldela licenser till användare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) och [tilldela licenser till användar konton med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="02426-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="02426-116">Microsoft Support tillhandahåller inte hjälp med att skapa skript, men dokumentation i licens tilldelning för Yammer är tillgänglig.</span><span class="sxs-lookup"><span data-stu-id="02426-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="02426-117">Mer information finns i [hantera Yammer-licenser med hjälp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="02426-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>