---
title: Aktivera tillbakaskrivning av lösenord i Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093373"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="04d00-102">Aktivera tillbakaskrivning av lösenord i Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="04d00-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="04d00-103">Om du vill aktivera självbetjäning för återställning av tillbakaskrivning av lösenord aktiverar du först alternativet för tillbakaskrivning i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="04d00-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="04d00-104">Gå igenom följande steg från Azure AD Connect-servern:</span><span class="sxs-lookup"><span data-stu-id="04d00-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="04d00-105">Logga in på Azure AD Connect-servern och starta **konfigurations guiden för Azure AD Connect** .</span><span class="sxs-lookup"><span data-stu-id="04d00-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="04d00-106">På **Välkomstsidan** klickar du på **Konfigurera**.</span><span class="sxs-lookup"><span data-stu-id="04d00-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="04d00-107">På sidan **Ytterligare tasks** klickar du på **Anpassa synkroniseringsalternativ** och sedan på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="04d00-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="04d00-108">På sidan **Anslut till Azure AD** skriver du dina globala administratörsautentiseringsuppgifter. Klicka sedan på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="04d00-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="04d00-109">På sidorna **Anslut kataloger** och **Domän-/OU-filtrering** klickar du på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="04d00-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="04d00-110">På sidan **Valfria funktioner** väljer du **Tillbakaskrivning av lösenord** och klickar på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="04d00-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="04d00-111">På sidan **Redo att konfigurera** klickar du på **Konfigurera** och väntar tills processen har slutförts.</span><span class="sxs-lookup"><span data-stu-id="04d00-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="04d00-112">När konfigurationen är klar klickar du på **Avsluta**.</span><span class="sxs-lookup"><span data-stu-id="04d00-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="04d00-113">Med tillbakaskrivning av lösenord aktiverat i Azure AD Connect konfigurerar du Azure AD-SSPR för tillbakaskrivning.</span><span class="sxs-lookup"><span data-stu-id="04d00-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="04d00-114">Om du vill aktivera tillbakaskrivning av lösen ord i SSPR gör du så här:</span><span class="sxs-lookup"><span data-stu-id="04d00-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="04d00-115">Logga in på Azure-portalen med ditt globala administratörskonto.</span><span class="sxs-lookup"><span data-stu-id="04d00-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="04d00-116">Sök efter och välj **Azure Active Directory**, klicka på **Återställ lösenord** och klicka sedan på **Lokal integration**.</span><span class="sxs-lookup"><span data-stu-id="04d00-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="04d00-117">Ange alternativet för **Skriv tillbaka lösenordet till din lokala katalog?** **Ja**.</span><span class="sxs-lookup"><span data-stu-id="04d00-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="04d00-118">Ställ in alternativet för **Tillåt användare att låsa upp konton utan att återställa deras lösen ord?** **Ja**.</span><span class="sxs-lookup"><span data-stu-id="04d00-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="04d00-119">När du är klar klickar du på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="04d00-119">When ready, click **Save**.</span></span>

<span data-ttu-id="04d00-120">Mer information finns i [Aktivera automatisk återställning av lösenord i Azure Active Directory – tillbakaskrivning i en lokal miljö](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="04d00-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="04d00-121">När en administratör återställer en användares lösenord i Azure-portalen, om användaren är federerad eller lösenordets-hash är synkroniserad, skrivs lösenordet tillbaka till lokalt.</span><span class="sxs-lookup"><span data-stu-id="04d00-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="04d00-122">Denna funktionalitet kräver Azure Premium-licens (P1 eller P2) och stöds för nuvarande inte i Office administrationsportalen.</span><span class="sxs-lookup"><span data-stu-id="04d00-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
