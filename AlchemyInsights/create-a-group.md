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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816390"
---
# <a name="create-a-group"></a>Skapa en grupp

I det här avsnittet beskrivs hur du skapar grupper.

**Behörighet att skapa en grupp**

Se till att du har behörighet att skapa en ny grupp. Globala administratörer kan inaktivera skapande av grupper i Azure-portalen eller åtkomstpanelen. Du kan behöva en administratör för att skapa den nya gruppen åt dig eller ge dig rätt behörigheter.

**Hantera behörigheter för att skapa grupper**

1. Globala administratörer kan hantera behörigheter för att skapa grupper (av säkerhetsrelaterade orsaker) eller Office 365-grupper som skapats i Azure-portalen eller åtkomstpanelen genom att välja alternativen "Användare kan skapa säkerhetsgrupper i Azure-portaler" eller "Användare kan skapa Office 365-grupper i Azure-portaler" i Alla grupper Allmänt  >  **(Inställningar)**.
2. Du kan också begränsa möjligheten att skapa grupper om du vill välja en grupp användare om du har en Azure Active Directory P1 Premium-licens.

**Inaktivera välkomstmeddelande för nya medlemmar i Office 365-grupper**

Välkomstmeddelandet som skickas till användare som läggs till i Office 365-grupper kan inaktiveras genom att ställa in **UnifiedGroupWelcomeMessageEnabled** till False i Powershell. Läs mer om den här inställningen [här](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

