---
title: Tilldela en granskningsloggroll i Säkerhets- och & Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526531"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Tilldela en granskningsloggroll i Säkerhets- och & Office 365

Om du vill söka i Office 365-granskningsloggen måste administratören  ha rollen Endast visningsloggar eller rollen Granskningsloggar i Exchange Online.  De här rollerna tilldelas rollgrupperna Efterlevnadshantering och Organisationshantering som standard. Globala administratörer i Office 365 och Microsoft 365 läggs automatiskt till som medlemmar i rollgruppen Organisationshantering.

Om du vill låta en användare söka med den lägsta nivån av behörighet  skapar du en  anpassad rollgrupp i Exchange Online, lägger till rollen Visningsbaserade granskningsloggar eller Granskningsloggar och lägger sedan till användaren som medlem i den nya rollgruppen.

Mer information finns i Hantera [rollgrupper i Exchange Online och](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) söka i [granskningsloggen i Säkerhets- & Efterlevnadscenter.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)