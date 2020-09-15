---
title: Begränsa åtkomst i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700473"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomst i SharePoint eller OneDrive

Det finns många sätt att begränsa åtkomsten till SharePoint Online/OneDrive-tjänster. Dessa olika åtkomst begränsningar beskrivs nedan. 

**Behörighets begränsning**

I SharePoint Online och OneDrive för företag är det bara att begränsa åtkomsten till objekt som webbplatser, filer och mappar genom att bevilja åtkomst till de grupper/personer som ska ha åtkomst.

- [Anpassa behörigheter för en SharePoint-lista eller ett bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Anpassa behörigheter för SharePoint-webbplatser](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ändra behörigheter för en undermapp](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Styra åtkomsten från ohanterade enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint-eller global administratör kan du spärra eller begränsa åtkomsten till SharePoint-och OneDrive-innehåll från ohanterade enheter (de som inte är hybrid annonser eller kompatibla i Intune).

**Begränsning av nätverks plats**

Som IT-administratör kan du kontrol lera åtkomsten till SharePoint-och OneDrive-resurser baserat på definierade nätverks platser som du litar på. Detta kallas även platsbaserade principer. Mer information finns i [styra åtkomst till SharePoint Online-och OneDrive-data baserat på nätverks plats](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begränsning av webbplats lås** 

I SharePoint Online kan du låsa en webbplats samling, så ingen har åtkomst till. Detta ställs in via PowerShell och [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) med egenskapen [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Hindra användare från att skapa webbplatser eller under webbplatser**

Som SharePoint-administratör eller global administratör kan du låta användarna skapa och administrera sina egna SharePoint-webbplatser, bestämma vilka typer av webbplatser de kan skapa och ange plats för webbplatserna. Mer information finns i [Hantera webbplats skapande i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

