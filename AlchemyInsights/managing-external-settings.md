---
title: Hantera externa inställningar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294432"
---
# <a name="managing-external-settings"></a><span data-ttu-id="9e750-102">Hantera externa inställningar</span><span class="sxs-lookup"><span data-stu-id="9e750-102">Managing External Settings</span></span>

<span data-ttu-id="9e750-103">**Meddelande**</span><span class="sxs-lookup"><span data-stu-id="9e750-103">**Announcement**</span></span>

- <span data-ttu-id="9e750-104">[Utfasning av WebView-inloggningssupport från Google från den 4 januari 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="9e750-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="9e750-105">Testa om dina appar påverkas av att följa Googles anvisningar om kompatibilitetstestning</span><span class="sxs-lookup"><span data-stu-id="9e750-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="9e750-106">Se till att du använder systemets webbvy eller systemwebbläsare när du loggar in dina användare med Google-konsumentkonton</span><span class="sxs-lookup"><span data-stu-id="9e750-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="9e750-107">**Hantera inställningar för inbjudan**</span><span class="sxs-lookup"><span data-stu-id="9e750-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="9e750-108">Bekräfta att du [har konfigurerat inställningarna för externt samarbete så](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) att rätt personer kan skicka inbjudningar.</span><span class="sxs-lookup"><span data-stu-id="9e750-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="9e750-109">**Hantera behörigheter för gästanvändare**</span><span class="sxs-lookup"><span data-stu-id="9e750-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="9e750-110">Globala administratörer kan hantera gäståtkomstbehörigheter i katalogen via Azure Portal genom att konfigurera behörigheter för gäståtkomst på sidan Inställningar för externt samarbete.</span><span class="sxs-lookup"><span data-stu-id="9e750-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="9e750-111">[Läs mer om den här inställningen.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="9e750-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="9e750-112">Om du vill att dina gäster ska få åtkomst till appar som Teams eller SharePoint bekräftar du att du har konfigurerat apparna för att tillåta gäståtkomst.</span><span class="sxs-lookup"><span data-stu-id="9e750-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="9e750-113">Läs mer om [Teams inställningar och](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="9e750-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9e750-114">**Konfigurera inbjudningar:**</span><span class="sxs-lookup"><span data-stu-id="9e750-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="9e750-115">Aktivera B2B externt samarbete och hantera vem som kan bjuda in gäster</span><span class="sxs-lookup"><span data-stu-id="9e750-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9e750-116">Tillåta eller blockera inbjudningar till användare från specifika organisationer</span><span class="sxs-lookup"><span data-stu-id="9e750-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="9e750-117">**Konfigurera tillåtna identitetsproviders:**</span><span class="sxs-lookup"><span data-stu-id="9e750-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="9e750-118">Google-federation</span><span class="sxs-lookup"><span data-stu-id="9e750-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9e750-119">Direktfederation</span><span class="sxs-lookup"><span data-stu-id="9e750-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9e750-120">E-postautentisering med lösenord</span><span class="sxs-lookup"><span data-stu-id="9e750-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
