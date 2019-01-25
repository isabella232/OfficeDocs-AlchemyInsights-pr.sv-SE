---
title: 646 så här konfigurerar du AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499688"
---
# <a name="configure-sync-features"></a><span data-ttu-id="53066-102">Konfigurera synkroniseringsfunktioner</span><span class="sxs-lookup"><span data-stu-id="53066-102">Configure sync features</span></span>

<span data-ttu-id="53066-p101">Azure AD Anslut innehåller flera funktioner som har aktiverats som standard eller som du kan aktivera senare. Vissa funktioner kräver ytterligare konfigurering i specifika miljöer.</span><span class="sxs-lookup"><span data-stu-id="53066-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="53066-p102">Gränser för [filtrera](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekten synkroniseras till Azure AD. Som standard alla användare, kontakter, grupper, och Windows 10 är datorkonton synkroniserade. Du kan inkludera eller exkludera objekt baserat på andra attribut, domäner eller organisationsenheter.</span><span class="sxs-lookup"><span data-stu-id="53066-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="53066-p103">[Synkronisering av lösenord hash-](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösenord hash från lokal Active Directory till Azure AD. Detta kan lösenordshantering på en plats, men användning av samma lösenord i båda lokal och moln miljöer. Eftersom Active Directory är den auktoritära källan, kan du använda din egen lösenordsprinciper.</span><span class="sxs-lookup"><span data-stu-id="53066-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="53066-111">[(SSPR) för återställning av lösenord för självbetjäning](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösenord i molnet samtidigt som du fortfarande använder din lokala lösenordsprincip.</span><span class="sxs-lookup"><span data-stu-id="53066-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="53066-112">[Enheten tillbakaskrivning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) tillåter registrerade enheter i Azure AD ska skrivas tillbaka till lokal Active Directory så att de kan användas för villkorad tillgång.</span><span class="sxs-lookup"><span data-stu-id="53066-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="53066-p104">[Hindra oavsiktliga borttagningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverad som standard för att förhindra borttagning av för många samtidiga objekt (mer än 500 objekt per synkronisering). Du kan ändra den här inställningen för att uppfylla behoven för din organisation.</span><span class="sxs-lookup"><span data-stu-id="53066-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="53066-115">[Den automatiska uppgraderingen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverad som standard för express installationer och ser till att din version av Azure AD Anslut alltid är aktuella.</span><span class="sxs-lookup"><span data-stu-id="53066-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

