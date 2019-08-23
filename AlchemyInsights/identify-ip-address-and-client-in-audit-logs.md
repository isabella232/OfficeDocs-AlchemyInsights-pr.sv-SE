---
title: Identifiera IP-adressen och klienten i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539047"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ba78c-102">Identifiera IP-adressen och klienten i granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="ba78c-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ba78c-103">IP-adress som motsvarar en aktivitet av Office 365-användare eller administratör visas i granskningsloggarna.</span><span class="sxs-lookup"><span data-stu-id="ba78c-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ba78c-104">Klientinformation loggas också.</span><span class="sxs-lookup"><span data-stu-id="ba78c-104">The client information is also logged.</span></span> <span data-ttu-id="ba78c-105">Här är stegen för att identifiera sådan information</span><span class="sxs-lookup"><span data-stu-id="ba78c-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ba78c-106">Logga in på [Office 365 säkerhet & regelefterlevnadscentret](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ba78c-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ba78c-107">Gå till **Sök** > **Granska loggen** söksida.</span><span class="sxs-lookup"><span data-stu-id="ba78c-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ba78c-108">Om du är intresserad av en viss aktivitet, markerar du den i listan **aktiviteter** .</span><span class="sxs-lookup"><span data-stu-id="ba78c-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ba78c-109">Annars returneras alla aktiviteter för den valda användaren (standardinställning).</span><span class="sxs-lookup"><span data-stu-id="ba78c-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ba78c-110">**Obs**: vissa aktiviteter kanske inte är tillgängliga i menyn **aktiviteter** . men de granska objekt returneras om **Visa resultat för alla aktiviteter** är markerad (standard).</span><span class="sxs-lookup"><span data-stu-id="ba78c-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ba78c-111">Ange användarnamnet i fältet **användare** , Välj lämpligt datumintervall för aktiviteten och klicka sedan på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="ba78c-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ba78c-112">I resultatet ser du IP-adressen för den aktiviteten i resultatfönstret.</span><span class="sxs-lookup"><span data-stu-id="ba78c-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ba78c-113">Markera granskningsposten se detaljerad information i **information** utfällbar meny (t ex klient, användaren som utförde åtgärden osv.).</span><span class="sxs-lookup"><span data-stu-id="ba78c-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ba78c-114">Mer information finns i [söka efter IP-adressen för den dator som används för åtkomst till eventuella skador](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="ba78c-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
