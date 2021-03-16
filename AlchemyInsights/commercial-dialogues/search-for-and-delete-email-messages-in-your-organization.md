---
title: Söka efter och ta bort e-postmeddelanden i organisationen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750018"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="0050b-102">Söka efter och ta bort e-postmeddelanden i organisationen</span><span class="sxs-lookup"><span data-stu-id="0050b-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="0050b-103">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="0050b-103">Follow these steps:</span></span>

1. <span data-ttu-id="0050b-104">Om du inte är global administratör måste du lägga till ditt konto i rollgruppen **för eDiscovery-hanteraren** eller rollen För efterlevnadssökning för att söka efter **meddelanden.**</span><span class="sxs-lookup"><span data-stu-id="0050b-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="0050b-105">Om du vill ta bort meddelanden måste du gå med i **rollgruppen Organisationshantering** eller rollen **För hantering av sökning och rensning.**</span><span class="sxs-lookup"><span data-stu-id="0050b-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="0050b-106">Behörigheter till de här rollerna tilldelas [i Säkerhets- & säkerhets- och efterlevnadscenter.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="0050b-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="0050b-107">[Skapa en innehållssökning för](https://docs.microsoft.com/office365/securitycompliance/content-search) att hitta det meddelande du vill ta bort.</span><span class="sxs-lookup"><span data-stu-id="0050b-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="0050b-108">[Anslut till Säkerhets- & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0050b-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="0050b-109">Om du använder MFA kan du läsa följande instruktioner: Ansluta till Säkerhets- och [& Efterlevnadscenter med flerfaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0050b-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="0050b-110">Ta bort meddelandet: kör `New-ComplianceSearchAction` cmdleten för att ta bort meddelandet.</span><span class="sxs-lookup"><span data-stu-id="0050b-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="0050b-111">Borttagna meddelanden flyttas till en användares återställningsbara objekt-mapp.</span><span class="sxs-lookup"><span data-stu-id="0050b-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="0050b-112">Ett exempelkommando finns i Steg [3: Ta bort meddelandet.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="0050b-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>