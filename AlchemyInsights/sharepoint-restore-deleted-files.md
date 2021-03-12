---
title: Återställa en borttaget fil eller mapp
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707540"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="b6752-102">Återställa en borttaget fil eller mapp</span><span class="sxs-lookup"><span data-stu-id="b6752-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="b6752-103">SharePoint Online behåller säkerhetskopior av allt innehåll under ytterligare 14 dagar efter att de tagits bort.</span><span class="sxs-lookup"><span data-stu-id="b6752-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="b6752-104">Om innehållet inte kan återställas via papperskorgen eller filåterställning kan administratören kontakta Microsoft Support för att begära återställning när som helst i 14-dagarsfönster.</span><span class="sxs-lookup"><span data-stu-id="b6752-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="b6752-105">Återställning från säkerhetskopior kan bara utföras för webbplatssamlingar och underwebbplatser, inte för enskilda filer, listor eller bibliotek.</span><span class="sxs-lookup"><span data-stu-id="b6752-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="b6752-106">När du tar bort ett objekt eller en webbplats från Sharepoint tas det inte omedelbart bort.</span><span class="sxs-lookup"><span data-stu-id="b6752-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="b6752-107">Borttagna objekt hamnar i papperskorgen under en viss tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="b6752-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="b6752-108">Under denna tid kan du återställa de objekt som du har tagit bort till deras ursprungliga plats.</span><span class="sxs-lookup"><span data-stu-id="b6752-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="b6752-109">Besök länkarna nedan om du vill ha mer information.</span><span class="sxs-lookup"><span data-stu-id="b6752-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="b6752-110">[Återställa objekt i papperskorgen för en SharePoint-webbplats.](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="b6752-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="b6752-111">Återställa borttagna filer eller mappar i OneDrive</span><span class="sxs-lookup"><span data-stu-id="b6752-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="b6752-112">Återställa en borttagna webbplatssamling (inklusive grupp, kommunikation och andra webbplatser)</span><span class="sxs-lookup"><span data-stu-id="b6752-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="b6752-113">Återställa en borttagna OneDrive-webbplats</span><span class="sxs-lookup"><span data-stu-id="b6752-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="b6752-114">Vid åtgärder för massåterkorg kan administratörer överväga att använda [SharePoint Online PNP.](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="b6752-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="b6752-115">**Funktionen Återställ filer**</span><span class="sxs-lookup"><span data-stu-id="b6752-115">**Files Restore feature**</span></span>

<span data-ttu-id="b6752-116">Om många av dina OneDrive- eller SharePoint-filer tas bort, skrivs över, skadas eller smittas med skadlig kod kan du återställa hela OneDrive- eller SharePoint-biblioteket till en föregående tid med hjälp av filåterställningsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="b6752-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="b6752-117">Återställa ett OneDrive-bibliotek</span><span class="sxs-lookup"><span data-stu-id="b6752-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="b6752-118">Återställa ett dokumentbibliotek</span><span class="sxs-lookup"><span data-stu-id="b6752-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

