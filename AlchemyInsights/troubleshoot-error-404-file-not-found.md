---
title: Felsöka felet 404, filen hittades inte
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: e76864949bde7230e63f509823ab1e3edf631388
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750109"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="33f85-102">Felsöka felet 404, filen hittades inte</span><span class="sxs-lookup"><span data-stu-id="33f85-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="33f85-103">Ett fel 404 tas emot när användare försöker komma åt en webbplats eller en fil i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="33f85-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="33f85-104">Det beror ofta på att en webbplats eller fil eller grupp får ett nytt namn, flyttats eller tagits bort.</span><span class="sxs-lookup"><span data-stu-id="33f85-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="33f85-105">Till exempel: användarna får ett 404-fel vid åtkomst till rot webbplats samlingen och det har tagits bort.</span><span class="sxs-lookup"><span data-stu-id="33f85-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="33f85-106">Så här löser du felet 404 för en webbplats som har bytt namn, flyttats eller tagits bort:</span><span class="sxs-lookup"><span data-stu-id="33f85-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="33f85-107">Information om klassiska webbplatser i det klassiska administrations centret finns i [återställa en borttagen webbplats samling](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="33f85-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="33f85-108">För moderna webbplatser (kommunikation, gruppanslutna eller andra platser) som finns i det nya administrations centret för SharePoint kan du läsa [och återställa borttagna webbplatser i det nya administrations centret för SharePoint](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span><span class="sxs-lookup"><span data-stu-id="33f85-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="33f85-109">Så här löser du felet 404 för en fil (eller ett annat objekt) som har bytt namn, flyttats eller tagits bort:</span><span class="sxs-lookup"><span data-stu-id="33f85-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="33f85-110">Gå till SharePoint-eller OneDrive-webbplatsen och Visa pappers korgen från webbplats innehållet.</span><span class="sxs-lookup"><span data-stu-id="33f85-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="33f85-111">Se [återställa objekt i pappers korgen på en SharePoint-webbplats](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span><span class="sxs-lookup"><span data-stu-id="33f85-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="33f85-112">Om du fortfarande inte hittar objektet du kan söka i gransknings loggen om loggning är aktiverat kan du [söka i gransknings loggen i Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="33f85-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Microsoft 365 Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>
