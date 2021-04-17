---
title: Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827556"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="aee21-102">Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell</span><span class="sxs-lookup"><span data-stu-id="aee21-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="aee21-103">I administrationscentret för Microsoft 365 går du till sidan Konfigurera domäner och väljer den domän som du använder för webbplatsen i  >  [](https://admin.microsoft.com/Adminportal#/Domains) listan över domäner.</span><span class="sxs-lookup"><span data-stu-id="aee21-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="aee21-104">Välj **+ Ny anpassad post** och ange följande:</span><span class="sxs-lookup"><span data-stu-id="aee21-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="aee21-105">Ange följande för **DNS-typ**: **A (adress)**</span><span class="sxs-lookup"><span data-stu-id="aee21-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="aee21-106">I **Värdnamn eller alias** skriver du in **@**</span><span class="sxs-lookup"><span data-stu-id="aee21-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="aee21-107">I **IP-adress** skriver du in den statiska IP-adress där webbplatsen finns för närvarande (till exempel 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="aee21-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="aee21-p101">Det måste vara en  *statisk*  IP-adress för webbplatsen, inte en  *dynamisk*  IP-adress.Kontrollera med webbplatsen som är värd för din webbplats för att se till att du kan få en statisk IP-adress till din offentliga webbplats.</span><span class="sxs-lookup"><span data-stu-id="aee21-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="aee21-110">Välj **Spara**.</span><span class="sxs-lookup"><span data-stu-id="aee21-110">Select **Save**.</span></span>

<span data-ttu-id="aee21-111">Du kan dessutom skapa en CNAME-post för att kunderna lättare ska kunna hitta till webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="aee21-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="aee21-112">Välj **+ Ny anpassad post** och ange följande:</span><span class="sxs-lookup"><span data-stu-id="aee21-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="aee21-113">Ange följande för **DNS-typ**: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="aee21-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="aee21-114">I **Värdnamn eller alias** skriver du in **www**</span><span class="sxs-lookup"><span data-stu-id="aee21-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="aee21-115">I **Pekar på adress** skriver du in det fullständiga domännamnet (FQDN) för webbplatsen (till exempel contoso.com).</span><span class="sxs-lookup"><span data-stu-id="aee21-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="aee21-116">Välj **Spara**.</span><span class="sxs-lookup"><span data-stu-id="aee21-116">Select **Save**.</span></span>
