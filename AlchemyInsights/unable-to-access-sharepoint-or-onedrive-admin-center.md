---
title: Det går inte att SharePoint eller OneDrive administrationscentret
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020462"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Det går inte att SharePoint eller OneDrive administrationscentret

- Om webbplatsen i administrationscentret för SharePoint eller OneDrive är otillgänglig kan det finnas ett tillfälligt problem med tjänsten, där användarna upplever upprepade fördröjningar eller navigeringsfel när de öppnar SharePoint webbplatser eller öppnar OneDrive innehåll. Titta på [instrumentpanelen för](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) tjänstens hälsa för att se om din organisation påverkas.

- Globala och SharePoint-administratörer måste tilldelas en SharePoint-licens. Nyligen skapade konton som precis har tilldelats en SharePoint-licens eller administratörsroll kan uppleva problem med att öppna SharePoint, som till exempel Åtkomst nekad eller Användaren hittades inte. Tillåt minst ett dygn för att synkroniseringen ska slutföras i våra system. Vi förstår att ett dygn kanske känns som en lång tid. I många fall arbetar vi redan med en lösning.

- Privileged Identity Management[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)användare kan få åtkomst nekad om fönstret med tillåten åtkomst är mycket litet, se Åtkomst nekas [till PIM-konton.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)