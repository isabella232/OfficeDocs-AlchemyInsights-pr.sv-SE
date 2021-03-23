---
title: Ändra Microsoft Edge med hjälp av datakatalogvariabler i stället för hårdkodade sökvägar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036858"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Ändra Microsoft Edge med hjälp av datakatalogvariabler i stället för hårdkodade sökvägar

Om du till exempel i Windows vill lagra profildata under en användares lokala programdata i stället för på standardplatsen ställer du in *UserDataDir-principen* på **${local_app_data}\Edge\Profile**.

Mer information finns i Skapa [microsoft Edge användardatakatalogvariabler](https://docs.microsoft.com/deployedge/microsoft-edge-policies).