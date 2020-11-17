---
title: Skapa en grupp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089177"
---
# <a name="create-a-group"></a>Skapa en grupp

I det här avsnittet beskrivs hur du skapar grupper.

**Behörighet att skapa en grupp**

Se till att du har behörighet att skapa en ny grupp. Globala administratörer kan inaktivera skapande av grupper i Azure Portal eller åtkomst panelen. Du kan behöva en administratör för att skapa den nya gruppen åt dig, eller ge dig lämpliga behörigheter.

**Hantera behörigheter för grupp skapande**

1. Globala administratörer kan hantera behörigheter för grupp skapande (av säkerhetsrelaterade skäl) eller Office 365-grupper som har skapats i Azure-portalen eller åtkomst panelen genom att välja "användare kan skapa säkerhets grupper i Azure-portaler" eller "användare kan skapa Office 365-grupper i Azure portaler" i **alla grupper**  >  **Allmänt (inställningar)**.
2. Du kan också begränsa grupp skapande för att välja en grupp användare om du har en Azure Active Directory P1 Premium-licens.

**Inaktiverar välkomst meddelande för nya Office 365-gruppmedlemmar**

Välkomst meddelandet som skickas till användare som har lagts till i Office 365 grupper kan inaktive ras genom att ange **UnifiedGroupWelcomeMessageEnabled** till falskt i PowerShell. Lär dig mer om den [här inställningen.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

