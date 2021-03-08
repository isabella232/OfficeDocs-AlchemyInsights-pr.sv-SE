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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="bad02-102">Tilldela en granskningsloggroll i Säkerhets- och & Office 365</span><span class="sxs-lookup"><span data-stu-id="bad02-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="bad02-103">Om du vill söka i Office 365-granskningsloggen måste administratören  ha rollen Endast visningsloggar eller rollen Granskningsloggar i Exchange Online. </span><span class="sxs-lookup"><span data-stu-id="bad02-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="bad02-104">De här rollerna tilldelas rollgrupperna Efterlevnadshantering och Organisationshantering som standard.</span><span class="sxs-lookup"><span data-stu-id="bad02-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="bad02-105">Globala administratörer i Office 365 och Microsoft 365 läggs automatiskt till som medlemmar i rollgruppen Organisationshantering.</span><span class="sxs-lookup"><span data-stu-id="bad02-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="bad02-106">Om du vill låta en användare söka med den lägsta nivån av behörighet  skapar du en  anpassad rollgrupp i Exchange Online, lägger till rollen Visningsbaserade granskningsloggar eller Granskningsloggar och lägger sedan till användaren som medlem i den nya rollgruppen.</span><span class="sxs-lookup"><span data-stu-id="bad02-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="bad02-107">Mer information finns i Hantera [rollgrupper i Exchange Online och](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) söka i [granskningsloggen i Säkerhets- & Efterlevnadscenter.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="bad02-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>