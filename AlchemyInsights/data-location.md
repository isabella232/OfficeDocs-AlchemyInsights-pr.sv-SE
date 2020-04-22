---
title: Plats för data
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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655300"
---
# <a name="data-location"></a>Plats för data

Du kan visa platsen för din klient i administrationscentret eller genom att ansluta till Exchange Online via PowerShell.


**Administrationscenter:**
1. Logga in på [administrationscentret](https://admin.microsoft.com/Adminportal/Home).
2. Välj profil **för inställningar** > **organisation**.
3. Under **Dataplats**väljer du **Visa information**.


**Powershell:**
1. Anslut till Exchange Online med Windows PowerShell.
2. Kör [cmdleten Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) för att visa en lista över klientens egenskaper. 
3. Titta på OrganisationenId egendom.

När du har dataplatsen för EXO och SPO kan du bestämma vilken dataplats för andra tjänster du kan använda från [där dina data finns](https://products.office.com/where-is-your-data-located).