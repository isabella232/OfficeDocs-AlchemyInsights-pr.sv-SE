---
title: Ändra Microsoft Edge med hjälp av data-katalogpartitioner i stället för hårdkodade-sökvägar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679153"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ändra Microsoft Edge med hjälp av data-katalogpartitioner i stället för hårdkodade-sökvägar

Om du till exempel använder Windows för att lagra profil data under en användares lokala program data i stället för på standard platsen ställer du in principen för **UserDataDir** på **$ {local_app_data} \Edge\Profile**. 

Mer information finns i [skapa Microsoft Edge user data Directory-variabler](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).