---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559895"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="16ab7-102">Begränsa åtkomsten i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="16ab7-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="16ab7-103">Det finns många sätt att begränsa åtkomsten till tjänster i SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="16ab7-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="16ab7-104">Nedan beskrivs dessa olika åtkomstmetoder för begränsning.</span><span class="sxs-lookup"><span data-stu-id="16ab7-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="16ab7-105">**Begränsning av behörighet**</span><span class="sxs-lookup"><span data-stu-id="16ab7-105">**Permission Restriction**</span></span>

<span data-ttu-id="16ab7-106">I SharePoint Online och OneDrive för företag kan begränsa vi åtkomsten till objekt som webbplatser, filer och mappar genom att bara bevilja åtkomst till de grupper/personer som ska ha åtkomst.</span><span class="sxs-lookup"><span data-stu-id="16ab7-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="16ab7-107">Anpassa behörigheter för en SharePoint-lista eller ett bibliotek</span><span class="sxs-lookup"><span data-stu-id="16ab7-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="16ab7-108">Anpassa behörigheter för SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="16ab7-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="16ab7-109">Ändra behörigheterna för en undermapp</span><span class="sxs-lookup"><span data-stu-id="16ab7-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="16ab7-110">Styra åtkomsten från ohanterade enheter</span><span class="sxs-lookup"><span data-stu-id="16ab7-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="16ab7-111">Som en SharePoint- eller global administratör i Office 365 kan du spärra eller begränsa åtkomst till SharePoint och OneDrive-innehåll från ohanterade enheter (de inte hybrid AD kopplade eller kompatibla i Intune).</span><span class="sxs-lookup"><span data-stu-id="16ab7-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="16ab7-112">**Plats nätverksbegränsning**</span><span class="sxs-lookup"><span data-stu-id="16ab7-112">**Network Location Restriction**</span></span>

<span data-ttu-id="16ab7-113">Som IT-administratör kan du styra åtkomsten till SharePoint och OneDrive resurser baserat på definierade nätverksplatser som du litar på.</span><span class="sxs-lookup"><span data-stu-id="16ab7-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="16ab7-114">Detta kallas även för plats-baserade principen.</span><span class="sxs-lookup"><span data-stu-id="16ab7-114">This is also known as location-based policy.</span></span> <span data-ttu-id="16ab7-115">Mer information finns i [Kontrollera åtkomst till SharePoint Online och OneDrive data baserat på nätverksplats](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="16ab7-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="16ab7-116">**Lås webbplatsbegränsning**</span><span class="sxs-lookup"><span data-stu-id="16ab7-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="16ab7-117">I SharePoint Online har du möjlighet att låsa en webbplatssamling så att ingen har tillträde.</span><span class="sxs-lookup"><span data-stu-id="16ab7-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="16ab7-118">Det här värdet via PowerShell och [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) med hjälp av egenskapen [Set SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="16ab7-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="16ab7-119">**Begränsa användare från att skapa webbplatser och underwebbplatser**</span><span class="sxs-lookup"><span data-stu-id="16ab7-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="16ab7-120">Du kan låta användarna skapa och administrera sina egna SharePoint-webbplatser, fastställa vilken typ av platser som de kan skapa, som en SharePoint-administratör eller Office 365 global administratör och ange platsen för webbplatser.</span><span class="sxs-lookup"><span data-stu-id="16ab7-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="16ab7-121">Mer information finns i [Hantera webbplatsutveckling i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="16ab7-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

