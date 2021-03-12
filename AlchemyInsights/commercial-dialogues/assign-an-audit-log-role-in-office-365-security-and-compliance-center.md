---
title: Tilldela en granskningsloggroll i Säkerhets- och efterlevnadscenter & Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749524"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Tilldela en granskningsloggroll i Säkerhets- och efterlevnadscenter & Office 365

För att söka i Office 365-granskningsloggen måste en administratör tilldelas rollen Endast visa granskningsloggar eller rollen Granskningsloggar i Exchange Online.   De här rollerna tilldelas rollgrupperna Efterlevnadshantering och Organisationshantering som standard. Globala administratörer i Office 365 och Microsoft 365 läggs automatiskt till som medlemmar i rollgruppen Organisationshantering.

Om du vill göra det möjligt för en användare att söka med den  lägsta nivån av  behörigheter skapar du en anpassad rollgrupp i Exchange Online, lägger till rollen Visnings endast granskningsloggar eller Granskningsloggar och lägger sedan till användaren som medlem i den nya rollgruppen.

Mer information finns i Hantera [rollgrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) och [Söka i granskningsloggen i Säkerhets- & Efterlevnadscenter.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)