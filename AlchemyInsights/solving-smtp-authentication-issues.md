---
title: Aktivera SMTP-autentisering och felsökning
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077669"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="d600c-102">Aktivera SMTP-autentisering och felsökning</span><span class="sxs-lookup"><span data-stu-id="d600c-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="d600c-103">Om du vill aktivera SMTP-autentisering för en postlåda eller om du får felet "Klienten är inte autentiserad", "Autentiseringen lyckades inte" eller "SmtpClientAuthentication" med koden 5.7.57 eller 5.7.3 eller 5.7.139 när du försöker vidarebefordra e-post genom att autentisera en enhet eller ett program med Microsoft 365 utför du följande tre åtgärder för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="d600c-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="d600c-104">Inaktivera [Azure-säkerhetsstandarder genom](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) att ändra **Aktivera standardinställningar för säkerhet** till **Nej.**</span><span class="sxs-lookup"><span data-stu-id="d600c-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="d600c-105">a.</span><span class="sxs-lookup"><span data-stu-id="d600c-105">a.</span></span> <span data-ttu-id="d600c-106">Logga in på Azure Portal som säkerhetsadministratör, villkorlig åtkomstadministratör eller global administratör.</span><span class="sxs-lookup"><span data-stu-id="d600c-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="d600c-107">b.</span><span class="sxs-lookup"><span data-stu-id="d600c-107">b.</span></span> <span data-ttu-id="d600c-108">Bläddra till Azure Active Directory > **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="d600c-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="d600c-109">c.</span><span class="sxs-lookup"><span data-stu-id="d600c-109">c.</span></span> <span data-ttu-id="d600c-110">Välj **Hantera säkerhetsstandarder.**</span><span class="sxs-lookup"><span data-stu-id="d600c-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="d600c-111">d.</span><span class="sxs-lookup"><span data-stu-id="d600c-111">d.</span></span> <span data-ttu-id="d600c-112">Ställ **in Aktivera säkerhetsstandarder** på **Nej.**</span><span class="sxs-lookup"><span data-stu-id="d600c-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="d600c-113">e.</span><span class="sxs-lookup"><span data-stu-id="d600c-113">e.</span></span> <span data-ttu-id="d600c-114">Välj **Spara**.</span><span class="sxs-lookup"><span data-stu-id="d600c-114">Select **Save**.</span></span>

2. <span data-ttu-id="d600c-115">[Aktivera sändning av klient-SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den licensierade postlådan.</span><span class="sxs-lookup"><span data-stu-id="d600c-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="d600c-116">a.</span><span class="sxs-lookup"><span data-stu-id="d600c-116">a.</span></span> <span data-ttu-id="d600c-117">I Administrationscenter för Microsoft 365 går du **till Aktiva** användare och väljer användaren.</span><span class="sxs-lookup"><span data-stu-id="d600c-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="d600c-118">b.</span><span class="sxs-lookup"><span data-stu-id="d600c-118">b.</span></span> <span data-ttu-id="d600c-119">Gå till fliken E-post och välj **Hantera e-postprogram** under **E-postprogram.**</span><span class="sxs-lookup"><span data-stu-id="d600c-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="d600c-120">d.</span><span class="sxs-lookup"><span data-stu-id="d600c-120">d.</span></span> <span data-ttu-id="d600c-121">Kontrollera att **Autentiserad SMTP är** markerat (aktiverat).</span><span class="sxs-lookup"><span data-stu-id="d600c-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="d600c-122">e.</span><span class="sxs-lookup"><span data-stu-id="d600c-122">e.</span></span> <span data-ttu-id="d600c-123">Välj **Spara ändringar**.</span><span class="sxs-lookup"><span data-stu-id="d600c-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="d600c-124">[Inaktivera Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) för den licensierade postlådan.</span><span class="sxs-lookup"><span data-stu-id="d600c-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="d600c-125">a.</span><span class="sxs-lookup"><span data-stu-id="d600c-125">a.</span></span> <span data-ttu-id="d600c-126">Gå till Administrationscenter för Microsoft 365 och välj Användare aktiva användare i den  >  **vänstra navigeringsmenyn.**</span><span class="sxs-lookup"><span data-stu-id="d600c-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="d600c-127">b.</span><span class="sxs-lookup"><span data-stu-id="d600c-127">b.</span></span> <span data-ttu-id="d600c-128">Välj **Multifaktorautentisering**.</span><span class="sxs-lookup"><span data-stu-id="d600c-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="d600c-129">c.</span><span class="sxs-lookup"><span data-stu-id="d600c-129">c.</span></span> <span data-ttu-id="d600c-130">Markera användaren och inaktivera **Multi-Factor Auth.**</span><span class="sxs-lookup"><span data-stu-id="d600c-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
