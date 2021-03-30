---
title: Konfigurera Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402459"
---
# <a name="configure-endpoint-dlp"></a>Konfigurera Endpoint DLP

Med Microsoft Endpoint DLP kan du utöka funktionerna för DLP-skydd och övervakning till känslig information på enheter med Windows 10. När enheter har registrerats i Enhetshantering kan du skapa DLP-principer för att upprätthålla skyddsåtgärder för objekt. Aktivitetsutforskaren kan användas för att övervaka aktiviteten för känsliga objekt. Mer information finns i [Registrering av enheter i Enhetshantering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Så här kommer du igång med Endpoint DLP:

- Se till att du har rätt SKU/prenumerationslicensiering. Mer information finns i [för SKU/prenumerationslicensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollera vilka behörigheter som krävs för att aktivera Enhetshantering, komma åt registreringssidan eller aktivera/inaktivera enhetsövervakning. Mer information finns i [Behörigheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Registrera enheter i Enhetshantering genom att följa proceduren för registrering av enheter. Om du saknar alternativet för enhetsregistrering (förhandsversion) under **Inställningar** för Microsoft 365 Efterlevnad, bekräftar du att du har rätt licens och behörigheter som nämns ovan. Mer information finns i [Registrering av enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Skapa DLP-principer för att skydda känsliga objekt. Mer information finns i [principscenarier för Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Mer information om Microsoft Endpoint DLP finns i [Mer information om dataförlustskydd för slutpunkt (förhandsversion) för Microsoft 365 ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Viktiga steg för datainsamling, om support krävs:**

1. Ladda ned förhandsversionen av MDATP-klientanalysprogrammet från [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Kör verktyget från cmd-fönstret som administratör:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Ange det antal minuter som krävs för att köra scenariot när du uppmanas att göra det med "Ange antalet minuter för att samla in spårningar: "
5. Kör scenariot

Ta emot zip-filen som ska ges till supportagenten.
