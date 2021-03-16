---
title: Ta bort bakgrundstjänsten för Microsoft Search i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816339"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Ta bort bakgrundstjänsten för Microsoft Search i Bing

Om du vill ta bort bakgrundstjänsten för Microsoft Search i Bing kan du prova följande:

1. Så här återgår du till de ursprungliga inställningarna för sökmotor:

    a. Inaktivera **Använd Bing som [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) standardsökmotor.**

    b. [Gå till administrationscentret för Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) och avmarkera inställningen som påverkar alla användare i organisationen.

2. Så här tar du bort bakgrundstjänsten från en enskild enhet:

    a. Välj **Kontrollpanelen i > Program > Program och funktioner**.

    b. Högerklicka på **Microsoft Search i Bing** under listan över installerade program och klicka sedan på **Avinstallera**.

3. Om du vill ta bort bakgrundstjänsten från flera enheter i organisationen loggar du in som administratör och kör följande kommando i ett skript: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
