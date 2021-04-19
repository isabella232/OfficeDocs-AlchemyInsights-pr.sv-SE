---
title: Kontrollera åtkomst till gemensamma mappar med Hjälp av Outlook
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816758"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrollera åtkomst till gemensamma mappar med Hjälp av Outlook

Så här styr du vilka användare som kan komma åt gemensamma mappar i Outlook:

1. Använd `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Tillåta användare åtkomst till gemensamma mappar i Outlook  
$false: Förhindra att användare kommer åt gemensamma mappar i Outlook. Det här är standardvärdet.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Obs! Den här proceduren kan bara styra anslutningar med Outlook för Windows-klienter. Användare kan fortsätta komma åt gemensamma mappar med hjälp av OWA eller Outlook för Mac.

Mer information finns i [Kontrollerade anslutningar till gemensamma mappar i Outlook.](https://aka.ms/controlpf)
