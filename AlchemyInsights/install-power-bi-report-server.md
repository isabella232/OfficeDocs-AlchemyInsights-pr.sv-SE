---
title: Installera Power BI-rapportserver
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
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832112"
---
# <a name="install-power-bi-report-server"></a>Installera Power BI-rapportserver

1. Hitta platsen för PowerBIReportServer.exe och starta installationsprogrammet.

2. Välj **Installera Power BI Report Server**.

3. Välj en version att installera och välj sedan **Nästa**.

4. Du kan välja antingen Utvärdering eller Developer Edition i listrutan.  Annars kan du ange en produktnyckel för servern som du har skaffat från antingen Power BI-tjänsten eller Volume License Service Center. Mer information om hur du får en produktnyckel finns i avsnittet Innan du börjar. Läs och godkänn licensvillkoren och välj sedan **Nästa.**

5. Du måste ha en databasmotorn tillgänglig för att kunna lagra rapportserverdatabasen. Välj **Nästa** för att endast installera rapportservern.

6. Ange installationsplatsen för rapportservern. Välj **Installera för** att fortsätta.

7. När konfigurationen är lyckad väljer du **Konfigurera rapportserver för** att starta Reporting Services Configuration Manager.

Du behöver inte en SQL Server Database Engine-server som är tillgänglig när du installerar. Du behöver en för att konfigurera Reporting Services efter installationen.

Mer information: https://docs.microsoft.com/power-bi/report-server/install-report-server
