---
title: Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506425"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell

1. Markera den domän som du använder för din webbplats i listan över domäner på sidan [domäner](https://portal.office.com/adminportal/home#/Domains) .

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
