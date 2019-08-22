---
title: Felsöka Lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533825"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ec48b-102">Felsöka Lösenordssynkronisering</span><span class="sxs-lookup"><span data-stu-id="ec48b-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ec48b-103">Felsökning av problem där inga lösenord är synkroniserade med Azure AD Connect version 1.1.614.0 eller senare:</span><span class="sxs-lookup"><span data-stu-id="ec48b-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="ec48b-104">Öppna en ny Windows PowerShell-session på Azure AD Connect-servern med alternativet **Kör som administratör** .</span><span class="sxs-lookup"><span data-stu-id="ec48b-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="ec48b-105">Kör **Ange körningsprincipen RemoteSigned** eller **Ange körningsprincipen obegränsad**.</span><span class="sxs-lookup"><span data-stu-id="ec48b-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="ec48b-106">Starta guiden Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ec48b-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="ec48b-107">Gå till sidan **Fler aktiviteter** och välj **Felsök**klickar du på **Nästa**.</span><span class="sxs-lookup"><span data-stu-id="ec48b-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="ec48b-108">Klicka på **Starta för att starta felsökning** -menyn i PowerShell på sidan felsökning.</span><span class="sxs-lookup"><span data-stu-id="ec48b-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="ec48b-109">På huvudmenyn väljer du **Felsöka Lösenordssynkronisering**.</span><span class="sxs-lookup"><span data-stu-id="ec48b-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="ec48b-110">Sub-menyn väljer du **Lösenordssynkronisering fungerar inte alls**.</span><span class="sxs-lookup"><span data-stu-id="ec48b-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="ec48b-111">**Förstå resultaten av felsökning aktivitet**</span><span class="sxs-lookup"><span data-stu-id="ec48b-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="ec48b-112">Felsökning uppgift utför följande kontroller:</span><span class="sxs-lookup"><span data-stu-id="ec48b-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="ec48b-113">Kontrollerar att funktionen för synkronisering av lösenord är aktiverat för Azure AD-innehavare.</span><span class="sxs-lookup"><span data-stu-id="ec48b-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="ec48b-114">Verifierar att Azure AD Connect-servern inte är i läget för mellanlagring.</span><span class="sxs-lookup"><span data-stu-id="ec48b-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="ec48b-115">För varje befintlig lokal Active Directory connector (som motsvarar en befintlig Active Directory-skog):</span><span class="sxs-lookup"><span data-stu-id="ec48b-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="ec48b-116">Kontrollerar att funktionen för synkronisering av lösenord är aktiverat.</span><span class="sxs-lookup"><span data-stu-id="ec48b-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="ec48b-117">Söker efter lösenord synkronisering heartbeat händelser i händelseloggarna för Windows-program.</span><span class="sxs-lookup"><span data-stu-id="ec48b-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="ec48b-118">För varje Active Directory-domän under lokal Active Directory-anslutningen:</span><span class="sxs-lookup"><span data-stu-id="ec48b-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="ec48b-119">Verifierar att domänen kan nås från Azure AD Connect-servern.</span><span class="sxs-lookup"><span data-stu-id="ec48b-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="ec48b-120">Verifierar att Active Directory DS (AD DS)-konton som används av lokal Active Directory-anslutningen har rätt användarnamn, lösenord och behörigheter som krävs för synkronisering av lösenord.</span><span class="sxs-lookup"><span data-stu-id="ec48b-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="ec48b-121">Mer hjälp med felsökning av synkronisering av lösenord, finns i [Felsöka Lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ec48b-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  