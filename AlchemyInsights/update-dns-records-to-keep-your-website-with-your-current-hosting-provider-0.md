---
title: Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815803"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell

1. I administrations centret för Microsoft 365 går du till sidan **konfigurations**  >  [domäner](https://admin.microsoft.com/Adminportal#/Domains) och väljer den domän du använder för webbplatsen i listan över domäner.

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
