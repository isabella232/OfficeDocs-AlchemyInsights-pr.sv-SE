---
title: Problem med att återställa lösenord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696279"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="dc72d-102">Problem med att återställa lösenord</span><span class="sxs-lookup"><span data-stu-id="dc72d-102">Problems resetting password</span></span>

<span data-ttu-id="dc72d-103">Här är några av de problem som kan finnas när du återställer lösenordet och möjliga lösningar:</span><span class="sxs-lookup"><span data-stu-id="dc72d-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="dc72d-104">**Jag har ett problem med återställning av lösenord som inte omfattas av de andra kategorierna**</span><span class="sxs-lookup"><span data-stu-id="dc72d-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="dc72d-105">Se till att du har behörighet att återställa lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="dc72d-106">Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="dc72d-107">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="dc72d-108">Se till att du förstår licenskraven:</span><span class="sxs-lookup"><span data-stu-id="dc72d-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="dc72d-109">Du måste ha minst en tilldelad licens i organisationen</span><span class="sxs-lookup"><span data-stu-id="dc72d-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="dc72d-110">Endast användare i molnet – betald Office 365-SKU (O365) eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="dc72d-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="dc72d-111">Molnanvändare och/eller lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="dc72d-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="dc72d-112">Mer information om licenskrav finns i artikeln [Licenskrav för självbetjäning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)för återställning av lösenord i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc72d-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="dc72d-113">**Jag har problem med att testa principen för återställning av lösenord som jag har angett**</span><span class="sxs-lookup"><span data-stu-id="dc72d-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="dc72d-114">Nyligen använda principer kan ta flera minuter att replikera över alla datacenter och ändpunkter.</span><span class="sxs-lookup"><span data-stu-id="dc72d-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="dc72d-115">Det fysiska avståndet från datacentret påverkar också hur snabbt ändringar tillämpas.</span><span class="sxs-lookup"><span data-stu-id="dc72d-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="dc72d-116">Testa med en slutanvändare, inte en administratör, och pilottesta med en liten uppsättning användare.</span><span class="sxs-lookup"><span data-stu-id="dc72d-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="dc72d-117">Principerna som konfigurerats i Azure-portalen gäller ENDAST för slutanvändare, inte administratörer.</span><span class="sxs-lookup"><span data-stu-id="dc72d-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="dc72d-118">Microsoft tillämpar en stark standardprincip med tvådelar för återställning av lösenord för alla Azure-administratörsroller (exempel: global administratör, supportadministratör, lösenordsadministratör osv.)</span><span class="sxs-lookup"><span data-stu-id="dc72d-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="dc72d-119">Läs mer om [principer för administratörer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="dc72d-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="dc72d-120">**Jag vill distribuera återställning av lösenord men jag vill inte göra så att användarna registrerar ytterligare säkerhetsinformation**</span><span class="sxs-lookup"><span data-stu-id="dc72d-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="dc72d-121">Fyll i data för användarna i förväg så att de inte behöver det!</span><span class="sxs-lookup"><span data-stu-id="dc72d-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="dc72d-122">– Som administratör kan du ange telefon- och e-postegenskaper för användarna innan du distribuerar lösenordsåterställning till din organisation.</span><span class="sxs-lookup"><span data-stu-id="dc72d-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="dc72d-123">Du kan göra detta med ett API, PowerShell eller Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="dc72d-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="dc72d-124">Mer information finns här:</span><span class="sxs-lookup"><span data-stu-id="dc72d-124">More information here:</span></span>
- [<span data-ttu-id="dc72d-125">Distribuera lösenordsåterställning utan att användare måste registrera sig</span><span class="sxs-lookup"><span data-stu-id="dc72d-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="dc72d-126">Vilka data används vid återställning av lösenord</span><span class="sxs-lookup"><span data-stu-id="dc72d-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="dc72d-127">**Knappen för återställning av lösenord är nedtonad**</span><span class="sxs-lookup"><span data-stu-id="dc72d-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="dc72d-128">Du har inte behörighet att återställa den här användarens lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="dc72d-129">Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="dc72d-130">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="dc72d-131">**Jag ser inte bladet för återställning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="dc72d-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="dc72d-132">Du har inte behörighet att återställa lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="dc72d-133">Endast globala administratörer, lösenordsadministratörer och användaradministratörer kan återställa användarlösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="dc72d-134">Globala administratörer kan också återställa andra behöriga administratörers lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="dc72d-135">**Jag ser inte bladet för lokal integrering i lösenordsåterställning**</span><span class="sxs-lookup"><span data-stu-id="dc72d-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="dc72d-136">Det lokala integrationsbladet visas bara i hybridmiljöer , vilket innebär att du använder tillbakaskrivning av lösenord för att ändra lösenord för lokala användare.</span><span class="sxs-lookup"><span data-stu-id="dc72d-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="dc72d-137">Du ser inte det här bladet om:</span><span class="sxs-lookup"><span data-stu-id="dc72d-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="dc72d-138">Du använder inte tillbakaskrivning av lösenord</span><span class="sxs-lookup"><span data-stu-id="dc72d-138">You are not using password writeback</span></span>
    - <span data-ttu-id="dc72d-139">Det är ett problem med återskrivning av lösenord vid installation/anslutning</span><span class="sxs-lookup"><span data-stu-id="dc72d-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="dc72d-140">Det är problem med installation/anslutning av Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="dc72d-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="dc72d-141">Fler felsökningssteg för problem med tillbakaskrivning av lösenord finns i avsnittet [Felsöka tillbakaskrivning av lösenord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="dc72d-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="dc72d-142">**Jag vet inte hur jag återställer en användares lösenord**</span><span class="sxs-lookup"><span data-stu-id="dc72d-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="dc72d-143">Logga in på Azure-portalen som lämplig administratör.</span><span class="sxs-lookup"><span data-stu-id="dc72d-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="dc72d-144">Gå till bladet Användare och grupper och välj **Alla användare.**</span><span class="sxs-lookup"><span data-stu-id="dc72d-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="dc72d-145">Välj en användare i listan.</span><span class="sxs-lookup"><span data-stu-id="dc72d-145">Select a user from the list.</span></span>
1. <span data-ttu-id="dc72d-146">Välj Översikt för den valda användaren **och** klicka sedan på Återställ lösenord i **kommandofältet.**</span><span class="sxs-lookup"><span data-stu-id="dc72d-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="dc72d-147">Följ instruktionerna på skärmen.</span><span class="sxs-lookup"><span data-stu-id="dc72d-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="dc72d-148">Återställningar utförs endast via Azure Portal som har stöd för återställning av lösenord.</span><span class="sxs-lookup"><span data-stu-id="dc72d-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="dc72d-149">**Jag återställer en lokal användares lösenord från Office 365 Admin-portalen eller Office 365-mobilappen, men användaren kan fortfarande inte logga in**</span><span class="sxs-lookup"><span data-stu-id="dc72d-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="dc72d-150">Password Writeback stöds inte i den här portalen.</span><span class="sxs-lookup"><span data-stu-id="dc72d-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="dc72d-151">Återställ användarens lösenord igen i Azure Portal – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="dc72d-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

