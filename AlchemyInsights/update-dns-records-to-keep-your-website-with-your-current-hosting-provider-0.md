---
title: Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665778"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell

1. Gå till sidan **Setup**  >  [Installationsdomäner i administrationscentret](https://portal.office.com/adminportal/home#/Domains) för Microsoft 365 och välj den domän som du använder för webbplatsen i listan över domäner.

2. Välj **+ Ny anpassad post** och ange följande:

  - Ange följande för **DNS-typ**: **A (adress)**

  - I **Värdnamn eller alias** skriver du in **@**

  - I **IP-adress** skriver du in den statiska IP-adress där webbplatsen finns för närvarande (till exempel 172.16.140.1).

    Det måste vara en  *statisk*  IP-adress för webbplatsen, inte en  *dynamisk*  IP-adress.Kontrollera med webbplatsen som är värd för din webbplats för att se till att du kan få en statisk IP-adress till din offentliga webbplats.

3. Välj **Spara**.

Du kan dessutom skapa en CNAME-post för att kunderna lättare ska kunna hitta till webbplatsen.
  
1. Välj **+ Ny anpassad post** och ange följande:

  - Ange följande för **DNS-typ**: **CNAME (alias)**

  - I **Värdnamn eller alias** skriver du in **www**

  - I **Pekar på adress** skriver du in det fullständiga domännamnet (FQDN) för webbplatsen (till exempel contoso.com).

2. Välj **Spara**.
