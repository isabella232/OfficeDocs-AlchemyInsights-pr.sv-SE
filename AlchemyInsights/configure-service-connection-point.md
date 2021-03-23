---
title: Konfigurera SCP (Service Connection Point)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037290"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="a7ec7-102">Konfigurera SCP (Service Connection Point)</span><span class="sxs-lookup"><span data-stu-id="a7ec7-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="a7ec7-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="a7ec7-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="a7ec7-104">**Orsak:** Det går inte att läsa SCP-objektet och få information om Azure AD-klientorganisationen</span><span class="sxs-lookup"><span data-stu-id="a7ec7-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="a7ec7-105">**Lösning:** Se avsnittet Konfigurera [en tjänstanslutningspunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="a7ec7-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="a7ec7-106">**Handlingsplan**</span><span class="sxs-lookup"><span data-stu-id="a7ec7-106">**Action plan**</span></span>

- <span data-ttu-id="a7ec7-107">Kontrollera om enheten har fått GPO:t för kontrollerad verifiering.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="a7ec7-108">Kontrollera att GPO:t har skapat registernycklarna.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="a7ec7-109">Kontrollera att du har två nycklar skapade med ditt katalog-ID och onmicrosoft-domän.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="a7ec7-110">**Konfigurera registerinställning på klientsidan för SCP**</span><span class="sxs-lookup"><span data-stu-id="a7ec7-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="a7ec7-111">Använd följande exempel för att skapa ett grupprincipobjekt (GPO) för att distribuera en registerinställning som konfigurerar en SCP-post i registret på dina enheter.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="a7ec7-112">Öppna en konsol för hantering av grupprinciper och skapa ett nytt GPO på domänen.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="a7ec7-113">Ange ditt nya GPO ett namn (till exempel ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="a7ec7-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="a7ec7-114">Redigera GPO:t och leta reda på följande sökväg: **Datorkonfiguration > inställningar > Windows-> register**.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="a7ec7-115">Högerklicka på registret **och** välj Ny **> registerpost.**</span><span class="sxs-lookup"><span data-stu-id="a7ec7-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="a7ec7-116">På **fliken Allmänt** konfigurerar du följande:</span><span class="sxs-lookup"><span data-stu-id="a7ec7-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="a7ec7-117">**Åtgärd:** Uppdatera</span><span class="sxs-lookup"><span data-stu-id="a7ec7-117">**Action**: Update</span></span>
    
- <span data-ttu-id="a7ec7-118">**Registreringsdatafil**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="a7ec7-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="a7ec7-119">**Nyckelsökväg:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="a7ec7-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="a7ec7-120">**Värdenamn**: TenantId</span><span class="sxs-lookup"><span data-stu-id="a7ec7-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="a7ec7-121">**Värdetyp:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="a7ec7-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="a7ec7-122">**Värdedata:** GUID- eller katalog-ID för Azure AD-instansen (Det här värdet finns i **Azure Portal > Azure Active Directory > Egenskaper > Katalog-ID**)</span><span class="sxs-lookup"><span data-stu-id="a7ec7-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="a7ec7-123">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="a7ec7-124">Högerklicka på registret **och** välj Ny **> registerpost.**</span><span class="sxs-lookup"><span data-stu-id="a7ec7-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="a7ec7-125">På **fliken Allmänt** konfigurerar du följande:</span><span class="sxs-lookup"><span data-stu-id="a7ec7-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="a7ec7-126">**Åtgärd:** Uppdatera</span><span class="sxs-lookup"><span data-stu-id="a7ec7-126">**Action**: Update</span></span>
    
- <span data-ttu-id="a7ec7-127">**Registreringsdatafil**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="a7ec7-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="a7ec7-128">**Nyckelsökväg:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="a7ec7-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="a7ec7-129">**Värdenamn**: TenantName</span><span class="sxs-lookup"><span data-stu-id="a7ec7-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="a7ec7-130">**Värdetyp:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="a7ec7-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="a7ec7-131">**Värdedata:** Ditt verifierade domännamn om du använder federerad miljö, till exempel AD FS.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="a7ec7-132">Ditt verifierade domännamn eller ditt onmicrosoft.com (till exempel contoso.onmicrosoft).com om du använder hanterad miljö</span><span class="sxs-lookup"><span data-stu-id="a7ec7-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="a7ec7-133">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-133">Click **OK**.</span></span>

7. <span data-ttu-id="a7ec7-134">Stäng redigeraren för det nya GPO:t.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="a7ec7-135">Länka det nya GPO:t till önskad OU som innehåller domänbaserade datorer som tillhör din kontrollerade utrullningspopulation.</span><span class="sxs-lookup"><span data-stu-id="a7ec7-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="a7ec7-136">Mer information finns i [Kontrollerad validering av hybrid-AD-koppling för Azure – Azure AD | Microsoft-dokument och](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) [felsökningshybrid för Azure Active Directory-anslutna enheter | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)</span><span class="sxs-lookup"><span data-stu-id="a7ec7-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









