---
title: Skapa en grupp
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929323"
---
# <a name="create-a-group"></a>Skapa en grupp

I det här avsnittet beskrivs hur du skapar grupper.

**Behörighet att skapa en grupp**

Se till att du har behörighet att skapa en ny grupp. Globala administratörer kan inaktivera skapande av grupper i Azure-portalen eller åtkomstpanelen. Du kan behöva en administratör för att skapa den nya gruppen åt dig eller ge dig rätt behörigheter.

**Hantera behörigheter för att skapa grupper**

1. Globala administratörer kan hantera behörigheter för att skapa grupper (av säkerhetsrelaterade orsaker) eller Office 365-grupper som skapats i Azure-portalen eller åtkomstpanelen genom att välja "Användare kan skapa säkerhetsgrupper i Azure-portaler" eller "Användare kan skapa Office 365-grupper i Azure-portaler" i Alla grupper Allmänt  >  **(Inställningar)**.
2. Du kan också begränsa skapandet av grupper om du vill välja en grupp användare om du har en licens Azure Active Directory P1 Premium grupp.

**Inaktivera välkomstmeddelande för nya Office 365 gruppmedlemmar**

Välkomstmeddelandet som skickas till användare som läggs till i Office 365-grupper kan inaktiveras genom att ställa in **UnifiedGroupWelcomeMessageEnabled** till False i Powershell. Läs mer om den här inställningen [här](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

