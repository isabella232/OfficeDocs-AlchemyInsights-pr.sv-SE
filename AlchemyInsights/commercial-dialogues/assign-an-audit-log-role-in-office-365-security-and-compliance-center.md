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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="28337-102">Tilldela en granskningsloggroll i Säkerhets- och efterlevnadscenter & Office 365</span><span class="sxs-lookup"><span data-stu-id="28337-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="28337-103">För att söka i Office 365-granskningsloggen måste en administratör tilldelas rollen Endast visa granskningsloggar eller rollen Granskningsloggar i Exchange Online.  </span><span class="sxs-lookup"><span data-stu-id="28337-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="28337-104">De här rollerna tilldelas rollgrupperna Efterlevnadshantering och Organisationshantering som standard.</span><span class="sxs-lookup"><span data-stu-id="28337-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="28337-105">Globala administratörer i Office 365 och Microsoft 365 läggs automatiskt till som medlemmar i rollgruppen Organisationshantering.</span><span class="sxs-lookup"><span data-stu-id="28337-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="28337-106">Om du vill göra det möjligt för en användare att söka med den  lägsta nivån av  behörigheter skapar du en anpassad rollgrupp i Exchange Online, lägger till rollen Visnings endast granskningsloggar eller Granskningsloggar och lägger sedan till användaren som medlem i den nya rollgruppen.</span><span class="sxs-lookup"><span data-stu-id="28337-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="28337-107">Mer information finns i Hantera [rollgrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) och [Söka i granskningsloggen i Säkerhets- & Efterlevnadscenter.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="28337-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>