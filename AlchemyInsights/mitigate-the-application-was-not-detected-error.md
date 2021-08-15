---
title: Avhjälpa fel om att programmet inte identifierades
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026132"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Avhjälpa fel om att programmet inte identifierades

Installationsfelet ”Programmet kunde inte identifieras när installationen hade slutförts” som rapporteras av Intune kan uppstå på alla större operativsystemsplattformar (Windows, iOS och Android).

De vanligaste scenarier som genererar felet är:

- Appen har uppdaterats utanför Intune (via en appbutik från tredje part) efter den första distributionen. Vissa program, till exempel Google Chrome, kan utföra automatiska uppdateringar.
- En användare har avinstallerat appen efter den första installationen.

Om du vill avhjälpa problemet måste du först granska de berörda enheterna för att avgöra vilket scenario som orsakat felet.

- Om appen har uppdaterats utanför Intune kan programdistributionen ställas in att ignorera programversionen. Om du vill göra det går du till **Appkonfigurering > Appinformation** och ställer in **Ignorera appversion** på **Ja**.
- När det gäller klienten kan det vara lämpligt att appen distribueras ”efter behov” och att säkerställa att den senaste versionen distribueras.
- Alternativt kan du på iOS-plattformen använda funktionen för **automatisk uppdatering** som associeras med Apples volyminköpsprogram och som kan konfigureras så att den uppdateras automatiskt till nya appversioner när de blir tillgängliga.

Mer information om hur du felsöker problem med appinstallationer finns i [Felsöka problem med appinstallationer](https://docs.microsoft.com/intune/troubleshoot-app-install).
