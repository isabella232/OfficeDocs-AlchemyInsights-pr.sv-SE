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
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735160"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begränsa åtkomsten i SharePoint eller OneDrive

Det finns många sätt att begränsa åtkomsten till tjänster i SharePoint Online/OneDrive. Nedan beskrivs dessa olika åtkomstmetoder för begränsning. 

Begränsning av behörighet

I SharePoint Online och OneDrive för företag kan begränsa vi åtkomsten till objekt som webbplatser, filer och mappar genom att bara bevilja åtkomst till de grupper/personer som ska ha åtkomst.

[Anpassa behörigheter för en SharePoint-lista eller ett bibliotek](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Anpassa behörigheter för SharePoint-webbplats](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Ändra behörigheterna för en undermapp](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Styra åtkomsten från ohanterade enheter](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

Som en SharePoint- eller global administratör i Office 365 kan du spärra eller begränsa åtkomst till SharePoint och OneDrive-innehåll från ohanterade enheter (de inte hybrid AD kopplade eller kompatibla i Intune).

Plats nätverksbegränsning

Som IT-administratör kan du styra åtkomsten till SharePoint och OneDrive resurser baserat på definierade nätverksplatser som du litar på. Detta kallas även för plats-baserade principen. Mer information finns i [Kontrollera åtkomst till SharePoint Online och OneDrive data baserat på nätverksplats](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Lås webbplatsbegränsning 

I SharePoint Online har du möjlighet att låsa en webbplatssamling så att ingen har tillträde. Det här värdet via PowerShell och [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) med hjälp av egenskapen [Set SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.

Begränsa användare från att skapa webbplatser och underwebbplatser

Du kan låta användarna skapa och administrera sina egna SharePoint-webbplatser, fastställa vilken typ av platser som de kan skapa, som en SharePoint-administratör eller Office 365 global administratör och ange platsen för webbplatser. Mer information finns i [Hantera webbplatsutveckling i SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

