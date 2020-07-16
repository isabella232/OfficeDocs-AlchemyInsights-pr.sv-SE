---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148301"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="38787-102">Om identitet i Yammer</span><span class="sxs-lookup"><span data-stu-id="38787-102">About identity in Yammer</span></span>

<span data-ttu-id="38787-103">Vi rekommenderar att alla nätverk vidtar följande åtgärder för att undvika identitetsrelaterade problem:</span><span class="sxs-lookup"><span data-stu-id="38787-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="38787-104">Framtvinga Office 365-identitet efter etablering av Microsoft 365-konton för användare i Azure AD för att säkerställa att alla användare loggar in med sitt primära Microsoft 365-konto.</span><span class="sxs-lookup"><span data-stu-id="38787-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="38787-105">Mer information finns i [Framtvinga Office 365-identitet för Yammer-användare](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="38787-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="38787-106">Konsolidera flera Yammer-nätverk.</span><span class="sxs-lookup"><span data-stu-id="38787-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="38787-107">Äldre Yammer-konfigurationer gör det möjligt för flera Yammer-nätverk att anslutas till en klient.</span><span class="sxs-lookup"><span data-stu-id="38787-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="38787-108">Mer information finns i [Nätverksmigrering - Konsolidera flera Yammer-nätverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="38787-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="38787-109">Du kan också tillämpa licensiering för Yammer för att blockera användare från Yammer om de inte har en licens.</span><span class="sxs-lookup"><span data-stu-id="38787-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="38787-110">Mer information finns [i Hantera Yammer-användarlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="38787-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="38787-111">Slutligen granska användarlistan för äldre Yammer-nätverk och pausa äldre användare.</span><span class="sxs-lookup"><span data-stu-id="38787-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="38787-112">Vi rekommenderar att du pausar (inaktiverar) användare i stället för att ta bort dem, eftersom borttagningen är oåterkallelig.</span><span class="sxs-lookup"><span data-stu-id="38787-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="38787-113">Mer information finns [i Granska Yammer-användare i nätverk som är anslutna till Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) och [Ta bort användare](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="38787-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="38787-114">Genom att konfigurera Yammer med hjälp av dessa steg är du också redo att konfigurera Yammer-nätverket för inbyggt läge för Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="38787-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="38787-115">Mer information finns i [Konfigurera Yammer-nätverket för inbyggt läge för Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="38787-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>