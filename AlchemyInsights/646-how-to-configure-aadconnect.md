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
# <a name="configure-sync-features"></a>Konfigurera synkroniseringsfunktioner

Azure AD Anslut innehåller flera funktioner som har aktiverats som standard eller som du kan aktivera senare. Vissa funktioner kräver ytterligare konfigurering i specifika miljöer.
  
- Gränser för [filtrera](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekten synkroniseras till Azure AD. Som standard alla användare, kontakter, grupper, och Windows 10 är datorkonton synkroniserade. Du kan inkludera eller exkludera objekt baserat på andra attribut, domäner eller organisationsenheter. 
    
- [Synkronisering av lösenord hash-](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösenord hash från lokal Active Directory till Azure AD. Detta kan lösenordshantering på en plats, men användning av samma lösenord i båda lokal och moln miljöer. Eftersom Active Directory är den auktoritära källan, kan du använda din egen lösenordsprinciper. 
    
- [(SSPR) för återställning av lösenord för självbetjäning](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösenord i molnet samtidigt som du fortfarande använder din lokala lösenordsprincip. 
    
- [Enheten tillbakaskrivning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) tillåter registrerade enheter i Azure AD ska skrivas tillbaka till lokal Active Directory så att de kan användas för villkorad tillgång. 
    
- [Hindra oavsiktliga borttagningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverad som standard för att förhindra borttagning av för många samtidiga objekt (mer än 500 objekt per synkronisering). Du kan ändra den här inställningen för att uppfylla behoven för din organisation. 
    
- [Den automatiska uppgraderingen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverad som standard för express installationer och ser till att din version av Azure AD Anslut alltid är aktuella. 
    

