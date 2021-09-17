---
title: Användarbild visas fortfarande i Microsoft Teams organisationsschema
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422317"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Användarbild visas fortfarande i Microsoft Teams organisationsschema

Om en eller flera personer i organisationen har inaktiverats eller tagits bort och deras profilbild fortfarande visas i organisationsschemat är det möjligt att inställningen **ShowInAddressLists** är inställd på Falskt: 

1. Gå till Administrationscenter för Microsoft 365 > [Aktiva användare](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) och välj användaren med fotot som fortfarande visas. 
1. Välj fliken **E-post** och kontrollera att **Visa i global adresslista** är inställt på **Nej.**

Om inställningen **ShowInAddressLists** **till Nej** inte fungerar kontrollerar du följande: 

- Användaren kanske visas i mottagarlistan i Exchange. Mer information finns i [Hantera adresslistor i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Användaren kanske visas i adresslistan i Azure Active Directory. Mer information finns i [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 