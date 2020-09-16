---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664188"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="5af1e-102">Om identitet i Yammer</span><span class="sxs-lookup"><span data-stu-id="5af1e-102">About identity in Yammer</span></span>

<span data-ttu-id="5af1e-103">Alla nätverk bör vidtas för att undvika identitets problem:</span><span class="sxs-lookup"><span data-stu-id="5af1e-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="5af1e-104">Använd Office 365-identitet efter att ha etablerat Microsoft 365-konton för användare i Azure AD för att säkerställa att alla användare loggar in med sitt primära Microsoft-365-konto.</span><span class="sxs-lookup"><span data-stu-id="5af1e-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="5af1e-105">Mer information finns i [använda Office 365-identitet för Yammer-användare](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="5af1e-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="5af1e-106">Konsolidera flera Yammer-nätverk.</span><span class="sxs-lookup"><span data-stu-id="5af1e-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="5af1e-107">Tidigare Yammer-konfigurationer gör att flera Yammer-nätverk kan anslutas till en klient organisation.</span><span class="sxs-lookup"><span data-stu-id="5af1e-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="5af1e-108">Mer information finns i [klientmigrering: konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="5af1e-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="5af1e-109">Du kan också använda licensiering för Yammer för att blockera användare från Yammer om de inte har en licens.</span><span class="sxs-lookup"><span data-stu-id="5af1e-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="5af1e-110">Mer information finns i [hantera användar licenser för Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="5af1e-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="5af1e-111">Granska slutligen användar listan för äldre Yammer-nätverk och gör uppehåll för äldre användare.</span><span class="sxs-lookup"><span data-stu-id="5af1e-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="5af1e-112">Vi rekommenderar att du inaktiverar (inaktiverar) användare i stället för att ta bort dem, eftersom borttagningen inte kan ångras.</span><span class="sxs-lookup"><span data-stu-id="5af1e-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="5af1e-113">Mer information finns i [Granska Yammer-användare i nätverk anslutna till Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) och [ta bort användare](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="5af1e-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="5af1e-114">Genom att konfigurera Yammer med de här stegen kan du också konfigurera Yammer-nätverket för eget läge för Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5af1e-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="5af1e-115">Mer information finns i [Konfigurera ditt Yammer-nätverk för eget läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="5af1e-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>