---
title: Importera och exportera från Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037257"
---
# <a name="import-and-export-from-yammer"></a>Importera och exportera från Yammer

**Importera**

Alternativen för användarimport varierar beroende på om Yammer-nätverket är i [inbyggt läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller inte.

- **Icke-inbyggt läge:** Användare kan importeras till grupper med hjälp av Lägg till från adressbok [(begränsning](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) till 100 användare) i gruppinställningar eller i nätverket med [Massuppdatering](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) inom nätverksadministratören.
- **Inbyggt läge:** Åtgärder för gruppmedlemskap och nätverksmedlemskap ska utföras från [Microsoft 365-administratörsportalen,](https://docs.microsoft.com/microsoft-365/admin/add-users)Azure [AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ett annat Azure AD-alternativ. Nätverk i inbyggt läge har inte längre tillgång till Massuppdatering och andra äldre funktioner.

> [!IMPORTANT]
> Yammer hade aldrig stöd för import av innehåll från nätverksadministratören även när funktionen Dataexport användes i ett annat nätverk. Innehåll kan publiceras på nytt av partnerlösningar eller REST-API:er för Yammer.

**Exportera**

[Exportera nätverksdata inom nätverksadministratören](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillåter export av innehåll från Yammer-nätverk, inklusive meddelanden och filer. Bifogade filer kan vara extremt stora och exporter tar lång tid att slutföra. Vi rekommenderar att aktiva nätverk exporteras med API:t [för dataexport](https://developer.yammer.com/docs/data-export-api) i delar per dag eller vecka. Microsoft Support tillhandahåller inte egna skript för detta ändamål.

Det finns [en separat GDPR-export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) för att exportera innehåll för en enskild användare.