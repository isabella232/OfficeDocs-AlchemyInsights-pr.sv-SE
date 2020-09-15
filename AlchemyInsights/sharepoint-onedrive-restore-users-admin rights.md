---
title: Felsöka åtkomst nekade till OneDrive för företag-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670634"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Felsöka åtkomst nekade till OneDrive för företag-webbplatser

Det här problemet uppstår ofta när en användare tas bort och återskapas med samma huvud namn (UPN). Det nya kontot skapas med ett annat PUID-värde (unikt ID). När användaren försöker komma åt en webbplats samling eller deras OneDrive har användaren felaktigt PUID. Ett andra scenario inkluderar profilsynkronisering med en Active Directory-organisationsenhet (OU). Om användare redan har loggat in i SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan de uppleva det här problemet.

1. Lös problemet genom att återställa den ursprungliga UPN-filen enligt anvisningarna i artikeln [Återställ en användare i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen genom att följa de här stegen och [ta bort en användare från listan med användar information](). 
3. När det är klart kan du kontrol lera att användaren har administratörs behörighet för OneDrive-webbplatsen genom att följa anvisningarna för att [lägga till administratörens för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Mer information om behörighets nivåer finns i artikeln [förstå behörighets nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
