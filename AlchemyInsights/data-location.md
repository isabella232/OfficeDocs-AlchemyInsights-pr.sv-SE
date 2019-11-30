---
title: Data plats
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627864"
---
# <a name="data-location"></a>Data plats

Du kan visa platsen för din Office 365-klient i administratörscenter eller genom att ansluta till Exchange Online via PowerShell.


**Admin Center:**
1. Logga in på [administratörscenter](https://admin.microsoft.com/Adminportal/Home).
2. Välj **Inställningar** > **organisations profil**.
3. Under **data plats**väljer du **Visa information**.


**Powershell:**
1. Ansluta till Exchange Online med hjälp av Windows PowerShell.
2. Kör cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) om du vill visa en lista över klientens egenskaper. 
3. Titta på egenskapen OrganizationId.

När du har data platsen för EXO och SPO kan du bestämma data platsen för andra tjänster som du kan använda [varifrån dina data finns](https://products.office.com/where-is-your-data-located).