---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750682"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f290c-102">Begränsa åtkomsten i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="f290c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f290c-103">Det finns många sätt att begränsa åtkomsten till SharePoint Online/OneDrive-tjänster.</span><span class="sxs-lookup"><span data-stu-id="f290c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f290c-104">Dessa olika metoder för åtkomstbegränsning beskrivs nedan.</span><span class="sxs-lookup"><span data-stu-id="f290c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f290c-105">**Behörighetsbegränsning**</span><span class="sxs-lookup"><span data-stu-id="f290c-105">**Permission Restriction**</span></span>

<span data-ttu-id="f290c-106">I SharePoint Online och OneDrive för företag begränsar vi åtkomsten till objekt som webbplatser, filer och mappar genom att endast bevilja åtkomst till de grupper/personer som ska ha åtkomst.</span><span class="sxs-lookup"><span data-stu-id="f290c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f290c-107">Anpassa behörigheter för en SharePoint-lista eller-bibliotek</span><span class="sxs-lookup"><span data-stu-id="f290c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f290c-108">Anpassa SharePoint-webbplatbehörigheter</span><span class="sxs-lookup"><span data-stu-id="f290c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f290c-109">Ändra behörigheterna för en undermapp</span><span class="sxs-lookup"><span data-stu-id="f290c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f290c-110">Styra åtkomsten från ohanterade enheter</span><span class="sxs-lookup"><span data-stu-id="f290c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f290c-111">Som en SharePoint-eller global administratör i Office 365 kan du blockera eller begränsa åtkomsten till SharePoint-och OneDrive-innehåll från ohanterade enheter (de som inte är hybrid AD-anslutna eller kompatibla i Intune).</span><span class="sxs-lookup"><span data-stu-id="f290c-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f290c-112">**Begränsning av nätverksplats**</span><span class="sxs-lookup"><span data-stu-id="f290c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f290c-113">Som IT-administratör kan du styra åtkomsten till SharePoint-och OneDrive-resurser baserat på definierade nätverksplatser som du litar på.</span><span class="sxs-lookup"><span data-stu-id="f290c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f290c-114">Detta kallas även platsbaserad princip.</span><span class="sxs-lookup"><span data-stu-id="f290c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f290c-115">Mer information finns i [kontrollera åtkomsten till SharePoint Online-och OneDrive-data baserat på nätverksplats](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f290c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f290c-116">**Begränsning av webbplats lås**</span><span class="sxs-lookup"><span data-stu-id="f290c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f290c-117">I SharePoint Online har du möjlighet att låsa en webbplatssamling, så att ingen har åtkomst.</span><span class="sxs-lookup"><span data-stu-id="f290c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f290c-118">Detta anges via PowerShell och [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) med hjälp av den [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate egenskapen.</span><span class="sxs-lookup"><span data-stu-id="f290c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f290c-119">**Begränsa användare från att skapa webbplatser eller underwebbplatser**</span><span class="sxs-lookup"><span data-stu-id="f290c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f290c-120">Som SharePoint-administratör eller Office 365 global administratör kan du låta användarna skapa och administrera sina egna SharePoint-webbplatser, bestämma vilka typer av webbplatser de kan skapa och ange platsen för webbplatserna.</span><span class="sxs-lookup"><span data-stu-id="f290c-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f290c-121">Mer information finns [i Hantera webbplats skapas i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f290c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

