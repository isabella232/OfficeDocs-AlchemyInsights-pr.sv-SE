---
title: Loggar och rapportering
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036099"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="62476-102">Loggar och rapportering</span><span class="sxs-lookup"><span data-stu-id="62476-102">Logs and Reporting</span></span>

<span data-ttu-id="62476-103">[Vanliga frågor och svar om Azure Active Directory-rapportering](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) besvarar vanliga frågor och svar om Azure Active Directory-rapportering (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="62476-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="62476-104">Mer information finns i [Azure Active Directory-rapportering.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="62476-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="62476-105">**Felsöka problem med granskning**</span><span class="sxs-lookup"><span data-stu-id="62476-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="62476-106">Om du har problem med att se vissa granskningsaktiviteter och den saknade aktiviteten finns i den här [listan](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)kan du skicka ett supportärenden.</span><span class="sxs-lookup"><span data-stu-id="62476-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="62476-107">Om du har problem med att se granskningsloggar i klientorganisationen ska du lämna in ett supportärenden.</span><span class="sxs-lookup"><span data-stu-id="62476-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="62476-108">Om dina granskningsaktiviteter inte visas direkt i Azure [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Portal kan du ta en titta på vår svarstidsinformation och skapa ett support ärende om fördröjningen överskrider den dokumenterade svarstiden.</span><span class="sxs-lookup"><span data-stu-id="62476-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="62476-109">Bevarande av Azure AD-aktivitetsloggar</span><span class="sxs-lookup"><span data-stu-id="62476-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="62476-110">Om du inte ser alla granskningar för det valda datumintervallet kan du ladda ned upp till 250 000 rader (sorterade efter senaste) inloggningar från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="62476-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="62476-111">Mer information finns i ladda [ned granskningsaktiviteter.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="62476-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="62476-112">**Felsöka problem med inloggningar**</span><span class="sxs-lookup"><span data-stu-id="62476-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="62476-113">Du kan bara se de senaste 30 dagarna av data om du har en Azure AD Premium-licens (P1 eller P2) för klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="62476-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="62476-114">Inloggningar är endast tillgängliga för Azure AD Premium-klienter.</span><span class="sxs-lookup"><span data-stu-id="62476-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="62476-115">Det är inte tillgängligt för kostnadsfria eller grundläggande licensierade klientorganisationar.</span><span class="sxs-lookup"><span data-stu-id="62476-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="62476-116">Om klientorganisationen har en Premium P1-licens och du inte kan [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) se inloggningarna kan du ta en titta på vår svarstid och skapa ett supportavtal om fördröjningen överskrider den dokumenterade svarstiden.</span><span class="sxs-lookup"><span data-stu-id="62476-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="62476-117">Om du inte ser alla inloggningar för det valda datumintervallet kan du ladda ned upp till 250 000 rader (sorterade efter senaste) inloggningar från Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="62476-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="62476-118">Mer information finns i [nedladdningsaktiviteter för inloggning.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="62476-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="62476-119">**Felsöka säkerhetsrapporter (användare som är flaggade på risk, riskabel inloggning)**</span><span class="sxs-lookup"><span data-stu-id="62476-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="62476-120">Användare som har flaggats för risksäkerhetsrapport</span><span class="sxs-lookup"><span data-stu-id="62476-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="62476-121">Riskabel inloggningsrapport i Azure Active Directory-portalen</span><span class="sxs-lookup"><span data-stu-id="62476-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="62476-122">Azure Active Directory-riskhändelser</span><span class="sxs-lookup"><span data-stu-id="62476-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
