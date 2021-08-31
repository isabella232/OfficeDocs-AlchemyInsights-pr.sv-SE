---
title: Användarbild visas inte i Microsoft Teams organisationsschema
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792887"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Användarbild visas inte i Microsoft Teams organisationsschema

Om en eller flera personer i organisationen saknar profilfoto i organisationsschemat kan inställningen **ShowInAddressLists** vara inställd på **Falskt:**

1. Gå till Administrationscenter för Microsoft 365 > [**Aktiva användare**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)och välj den användare som saknar foto. 
1. Välj fliken **E-post** och kontrollera att **Visa i global adresslista** är inställt på **Ja.** 

Om det inte går att  ställa **in ShowInAddressLists** på Ja kontrollerar du följande:

- Användaren kan vara dold från mottagarlistan i Exchange. Mer information finns i [Hantera adresslistor i Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Användaren kan vara dold från adresslistan i Azure Active Directory. Mer information finns i [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
