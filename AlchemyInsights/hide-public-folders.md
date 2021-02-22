---
title: Dölj gemensamma mappar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315441"
---
# <a name="hide-public-folders"></a>Dölj gemensamma mappar

**Så här döljer du hela träd i den gemensamma mappen:**

Använd stegen i den [här artikeln](https://aka.ms/ControlPF) för att dölja hela offentliga mappträd för selektiva eller alla användare.

**Så här döljer du en specifik offentlig mapp:**

1. Lägga till behörigheter för användare som behöver åtkomst till den gemensamma mappen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Ta bort **användarens standard** från **behörighetslistan:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
