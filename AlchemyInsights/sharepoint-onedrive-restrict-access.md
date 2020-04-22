---
title: Begränsa åtkomsten i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692783"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomsten i SharePoint eller OneDrive

Det finns många sätt att begränsa åtkomsten till SharePoint Online/OneDrive-tjänster. Dessa olika metoder för åtkomstbegränsning beskrivs nedan. 

**Begränsning av behörighet**

I SharePoint Online och OneDrive för företag begränsar vi åtkomsten till objekt som webbplatser, filer och mappar genom att endast bevilja åtkomst till de grupper/personer som ska ha åtkomst.

- [Anpassa behörigheter för en SharePoint-lista eller ett SharePoint-bibliotek](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Anpassa behörigheter för SharePoint-webbplatser](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Ändra behörigheterna för en undermapp](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Styra åtkomsten från ohanterade enheter](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Som SharePoint- eller global administratör kan du blockera eller begränsa åtkomsten till SharePoint- och OneDrive-innehåll från ohanterade enheter (de som inte är hybrid-AD anslutna eller kompatibla i Intune).

**Begränsning av nätverksplats**

Som IT-administratör kan du styra åtkomsten till SharePoint- och OneDrive-resurser baserat på definierade nätverksplatser som du litar på. Detta kallas även platsbaserad princip. Mer information finns i [Kontrollera åtkomst till SharePoint Online- och OneDrive-data baserat på nätverksplats](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Begränsning av platslås** 

Inom SharePoint Online har du möjlighet att låsa en webbplatssamling, så ingen har tillgång. Detta anges via PowerShell och [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) med egenskapen [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Hindra användare från att skapa webbplatser eller underwebbplatser**

Som SharePoint-administratör eller Global administratör kan du låta användarna skapa och administrera sina egna SharePoint-webbplatser, bestämma vilken typ av webbplatser de kan skapa och ange platsen för webbplatserna. Mer information finns [i Hantera webbplatsskapande i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

