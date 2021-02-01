---
title: Problem med autentiseringsuppgifter
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063720"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="b21b6-102">Problem med autentiseringsuppgifter</span><span class="sxs-lookup"><span data-stu-id="b21b6-102">Issues with credentials</span></span>

<span data-ttu-id="b21b6-103">Microsofts identitetsplattform och inloggningsflödet för [OAuth 2.0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver hur du programmerar direkt mot OAuth 2.0-klientautentiseringsflödet.</span><span class="sxs-lookup"><span data-stu-id="b21b6-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="b21b6-104">**Hur hanterar jag lösenord eller certifikatautentiseringsuppgifter för ett program?**</span><span class="sxs-lookup"><span data-stu-id="b21b6-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="b21b6-105">I Azure CLI kan du använda autentiseringsuppgifter för [az ad-app](https://docs.microsoft.com/cli/azure/ad/app/credential) till att ta bort, lista eller återställa ett programs lösenord eller certifikatuppgifter.</span><span class="sxs-lookup"><span data-stu-id="b21b6-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="b21b6-106">**Hur återställer mina användare sina lösenord?**</span><span class="sxs-lookup"><span data-stu-id="b21b6-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="b21b6-107">Användare måste [registrera sig för självbetjäning för återställning](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) av lösenord innan de kan återställa sina lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="b21b6-108">När en användare har registrerat sig kan han eller hon följa anvisningarna i den här artikeln för att återställa lösenordet: Återställa lösenordet för [arbetet eller skolan.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="b21b6-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="b21b6-109">**Hur ändrar mina användare sina lösenord?**</span><span class="sxs-lookup"><span data-stu-id="b21b6-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="b21b6-110">Användare kan följa stegen i den här artikeln för att ändra sina lösenord: [Så här ändrar du ditt lösenord.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="b21b6-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="b21b6-111">De kan också [hantera applösenord för tvåstegsverifiering.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="b21b6-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="b21b6-112">**Användaren får ett felmeddelande när han eller hon ändrar eller återställer lösenordet**</span><span class="sxs-lookup"><span data-stu-id="b21b6-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="b21b6-113">Den här länken innehåller information om vanliga problem som kan uppstå när en användare försöker återställa sitt lösenord: [vanliga problem och deras lösningar](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="b21b6-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="b21b6-114">**Jag har problem med att återställa en användares lösenord**</span><span class="sxs-lookup"><span data-stu-id="b21b6-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="b21b6-115">Kontrollera att du har behörighet att återställa lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="b21b6-116">*Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.*</span><span class="sxs-lookup"><span data-stu-id="b21b6-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b21b6-117">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="b21b6-118">Se till att du förstår licenskraven:</span><span class="sxs-lookup"><span data-stu-id="b21b6-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="b21b6-119">Du måste ha minst en tilldelad licens i organisationen:</span><span class="sxs-lookup"><span data-stu-id="b21b6-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="b21b6-120">**Endast användare i molnet** – betald Office 365-SKU (O365) eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b21b6-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="b21b6-121">**Molnanvändare och/eller** lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="b21b6-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="b21b6-122">Mer information om licenskrav finns i [Licenskrav för självbetjäning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)för återställning av lösenord i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b21b6-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="b21b6-123">Om du vill återställa en användares lösenord måste du hitta användaren i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b21b6-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="b21b6-124">Klicka sedan på knappen "Återställ lösenord" i översiktsbladet för den användaren.</span><span class="sxs-lookup"><span data-stu-id="b21b6-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="b21b6-125">**Knappen för återställning av lösenord är nedtonad**</span><span class="sxs-lookup"><span data-stu-id="b21b6-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="b21b6-126">Du har inte behörighet att **återställa** den här användarens lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="b21b6-127">*Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.*</span><span class="sxs-lookup"><span data-stu-id="b21b6-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b21b6-128">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b21b6-129">**Jag ser inte bladet för återställning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="b21b6-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="b21b6-130">Du har inte behörighet att återställa lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="b21b6-131">*Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.*</span><span class="sxs-lookup"><span data-stu-id="b21b6-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b21b6-132">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b21b6-133">**Jag ser inte det lokala integrationsbladet i lösenordsåterställning**</span><span class="sxs-lookup"><span data-stu-id="b21b6-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="b21b6-134">Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lösenord för lokala användare.</span><span class="sxs-lookup"><span data-stu-id="b21b6-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="b21b6-135">Du ser inte det här bladet om:</span><span class="sxs-lookup"><span data-stu-id="b21b6-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="b21b6-136">Du använder inte tillbakaskrivning av lösenord</span><span class="sxs-lookup"><span data-stu-id="b21b6-136">You are not using password writeback</span></span>
  - <span data-ttu-id="b21b6-137">Det är ett problem med återskrivning av lösenord vid installation/anslutning</span><span class="sxs-lookup"><span data-stu-id="b21b6-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="b21b6-138">Det är problem med installation/anslutning av Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b21b6-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="b21b6-139">Mer felsökningssteg för problem med tillbakaskrivning av lösenord finns i Felsöka tillbakaskrivning [av lösenord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="b21b6-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="b21b6-140">**Jag vet inte hur jag återställer en användares lösenord**</span><span class="sxs-lookup"><span data-stu-id="b21b6-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="b21b6-141">Logga in på Azure-portalen som lämplig administratör.</span><span class="sxs-lookup"><span data-stu-id="b21b6-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="b21b6-142">Gå till **bladet Användare och** grupper och välj Alla **användare.**</span><span class="sxs-lookup"><span data-stu-id="b21b6-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="b21b6-143">Välj en användare i listan.</span><span class="sxs-lookup"><span data-stu-id="b21b6-143">Select a user from the list.</span></span>
4. <span data-ttu-id="b21b6-144">Välj Översikt för **den** valda användaren och sedan Återställ lösenord i **kommandofältet.**</span><span class="sxs-lookup"><span data-stu-id="b21b6-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="b21b6-145">Välj knappen **Återställ lösenord** och följ instruktionerna på skärmen.</span><span class="sxs-lookup"><span data-stu-id="b21b6-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="b21b6-146">Återställningar utförs endast via **Azure Portal som har stöd** för återställning av lösenord.</span><span class="sxs-lookup"><span data-stu-id="b21b6-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="b21b6-147">**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilappen, men användaren kan fortfarande inte logga in**</span><span class="sxs-lookup"><span data-stu-id="b21b6-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="b21b6-148">Password Writeback stöds inte i den här portalen.</span><span class="sxs-lookup"><span data-stu-id="b21b6-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="b21b6-149">Återställ användarens lösenord igen i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b21b6-149">Reset the user's password again in the Azure portal.</span></span>
