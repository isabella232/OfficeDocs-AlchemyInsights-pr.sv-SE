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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657947"
---
# <a name="configure-endpoint-dlp"></a>Konfigurera Endpoint DLP

Med Microsoft Endpoint DLP kan du utöka funktionerna för DLP-skydd och övervakning till känslig information på enheter med Windows 10. När enheter har registrerats i Enhetshantering kan du skapa DLP-principer för att upprätthålla skyddsåtgärder för objekt. Aktivitetsutforskaren kan användas för att övervaka aktiviteten för känsliga objekt. Mer information finns i [Registrering av enheter i Enhetshantering](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Så här kommer du igång med Endpoint DLP:

- Se till att du har rätt SKU/prenumerationslicensiering. Mer information finns i [för SKU/prenumerationslicensiering](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollera vilka behörigheter som krävs för att aktivera Enhetshantering, komma åt registreringssidan eller aktivera/inaktivera enhetsövervakning. Mer information finns i [Behörigheter](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Registrera enheter i Enhetshantering genom att följa proceduren för registrering av enheter. Mer information finns i [Registrering av enheter](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Skapa DLP-principer för att skydda känsliga objekt. Mer information finns i [principscenarier för Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Mer information om Microsoft Endpoint DLP finns i [Mer information om dataförlustskydd för slutpunkt (förhandsversion) för Microsoft 365 ](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Viktiga steg för datainsamling, om support krävs:**

1. Hämta [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Kör verktyget från cmd-fönstret som administratör:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. När du uppmanas **att göra det med Ange antalet minuter för att samla in spårningar:** anger du hur många minuter som behövs för att köra scenariot.
1. Kör scenariot.

Samla in zip-filens utdata som du vill ge till supportagenten.
