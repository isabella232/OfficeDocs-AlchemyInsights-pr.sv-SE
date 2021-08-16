---
title: Kontrollera åtkomst till gemensamma mappar med hjälp av Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032576"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollera åtkomst till gemensamma mappar med hjälp av Outlook

Så här styr du vilka användare som kan komma åt gemensamma mappar Outlook:

1. Använd `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Tillåt användare att använda gemensamma mappar i Outlook  
$false: Förhindra att användare kommer åt gemensamma mappar i Outlook. Det här är standardvärdet.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Obs! Den här proceduren kan bara styra anslutningar Outlook skrivbordet för Windows klienter. Användare kan fortsätta få åtkomst till gemensamma mappar med hjälp av OWA eller Outlook för Mac.

Mer information finns i [Styrda anslutningar till gemensamma mappar Outlook](https://aka.ms/controlpf) mer information.
