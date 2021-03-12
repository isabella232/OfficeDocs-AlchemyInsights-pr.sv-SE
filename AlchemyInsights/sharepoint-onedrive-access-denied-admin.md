---
title: Felsöka meddelanden om nekad åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707972"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="29d19-102">Felsöka meddelanden om nekad åtkomst i administrationscentret för Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="29d19-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="29d19-103">Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett administrationscenter för Sharepoint/OneDrive ska du se till att du tilldelar en [licens till användaren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="29d19-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="29d19-104">Om användaren har en licens bör du också kontrollera att de har [tilldelats en administratörsroll](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som kan komma åt administratörscentrat.</span><span class="sxs-lookup"><span data-stu-id="29d19-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="29d19-105">Det här problemet kan också uppstå när en användare tas bort och på nytt skapas med samma huvudnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="29d19-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="29d19-106">Det nya kontot skapas med ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="29d19-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="29d19-107">När användaren försöker komma åt en webbplatssamling eller OneDrive har användaren ett felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="29d19-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="29d19-108">I det andra scenariot ingår katalogsynkronisering med organisationsenheten Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="29d19-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="29d19-109">Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan OU och synkroniseras om med SharePoint kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="29d19-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="29d19-110">Lös problemet genom att återställa det ursprungliga UPN med stegen i artikeln Återställ [en användare i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="29d19-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="29d19-111">Obs! Om ett Administrationscenter för OneDrive eller SharePoint inte är tillgängligt för flera användare som tidigare har haft åtkomst kan det finnas ett tillfälligt problem med tjänsten.</span><span class="sxs-lookup"><span data-stu-id="29d19-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="29d19-112">[Kontrollera hälsoinstrumentpanelen för tjänster.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="29d19-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


