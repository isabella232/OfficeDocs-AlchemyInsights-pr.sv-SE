---
title: Lösenords tillbakaskrivning fungerar inte
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243524"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="efb35-102">Lösenords tillbakaskrivning fungerar inte</span><span class="sxs-lookup"><span data-stu-id="efb35-102">Password Writeback is not working</span></span>

<span data-ttu-id="efb35-103">**Jag har problem med att konfigurera tillbakaskrivning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="efb35-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="efb35-104">Tillbakaskrivning av lösenord är en premium-funktion.</span><span class="sxs-lookup"><span data-stu-id="efb35-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="efb35-105">Se till att du förstår licenskraven:</span><span class="sxs-lookup"><span data-stu-id="efb35-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="efb35-106">Du måste ha minst en tilldelad licens i organisationen</span><span class="sxs-lookup"><span data-stu-id="efb35-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="efb35-107">**Endast användare i molnet** – betald Office 365-SKU (O365) eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="efb35-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="efb35-108">**Molnanvändare och/eller** lokala användare – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="efb35-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="efb35-109">Mer information om licenskrav finns i [Licenskrav för självbetjäning för lösenordsåterställning i Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="efb35-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="efb35-110">Du har minst ett administratörskonto och ett testanvändarkonto med en av rätt licens.</span><span class="sxs-lookup"><span data-stu-id="efb35-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="efb35-111">Du måste ansluta Azure AD Connect till den primära domänkontrollant emulatorn för att lösenord ska kunna återställas.</span><span class="sxs-lookup"><span data-stu-id="efb35-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="efb35-112">Du kan konfigurera Azure AD Connect för användning av  en primär domänkontrollant genom att högerklicka på egenskaperna för Active Directory-synkroniseringskopplingen och sedan välja **konfigurera katalogpartitioner.**</span><span class="sxs-lookup"><span data-stu-id="efb35-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="efb35-113">Där kan du titta efter avsnittet **om anslutningsinställningar för domänkontrollanter** och markera kryssrutan som endast **heter använd önskade domänkontrollanter.**</span><span class="sxs-lookup"><span data-stu-id="efb35-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="efb35-114">Om det önskade DC:et inte är en PDC-emulator, kommer Azure AD Connect fortfarande att kontakta PDC för att få tillbaka lösenordet.</span><span class="sxs-lookup"><span data-stu-id="efb35-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="efb35-115">Återställning av lösenord har konfigurerats och aktiverats i klientorganisationen.</span><span class="sxs-lookup"><span data-stu-id="efb35-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="efb35-116">Mer information finns i Aktivera [att användare återställer sina Azure AD-lösenord.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="efb35-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="efb35-117">Kontrollera att administratörskontot som används för att aktivera Lösenords tillbakaskrivning är ett molnadministratörskonto (som skapats i Azure AD, inte lokalt AD)</span><span class="sxs-lookup"><span data-stu-id="efb35-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="efb35-118">Du har en lokal distribution av en ad eller flera skogar som kör Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de senaste service packen installerade</span><span class="sxs-lookup"><span data-stu-id="efb35-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="efb35-119">Du har Azure AD Connect-verktyget installerat och förberett AD-miljön för synkronisering med molnet.</span><span class="sxs-lookup"><span data-stu-id="efb35-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="efb35-120">Innan du testar tillbakaskrivning av lösenord ska du först slutföra en fullständig import och fullständig synkronisering från både AD och Azure AD i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="efb35-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="efb35-121">Mer information finns i hur du gör en [fullständig synkronisering och fullständig import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="efb35-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="efb35-122">**Jag har problem med anslutning för återskrivning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="efb35-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="efb35-123">Ladda ned och aktivera den senaste versionen av [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="efb35-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="efb35-124">Brandväggskonfiguration: Verktyget Azure AD Connect (1.1.443 och högre) behöver **utgående HTTPS-åtkomst** till:</span><span class="sxs-lookup"><span data-stu-id="efb35-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="efb35-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="efb35-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="efb35-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="efb35-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="efb35-127">Tillåt att inaktiva anslutningar bevaras i minst 2–3 minuter</span><span class="sxs-lookup"><span data-stu-id="efb35-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="efb35-128">**Jag har fortfarande problem med tillbakaskrivning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="efb35-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="efb35-129">Om du fortfarande har problem kan du prova att inaktivera och återaktivera tjänsten för återställning av lösenord i Azure AD Connect-verktyget</span><span class="sxs-lookup"><span data-stu-id="efb35-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="efb35-130">Mer information finns i hur du [inaktiverar och återaktiverar lösenords tillbakaskrivning](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="efb35-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
