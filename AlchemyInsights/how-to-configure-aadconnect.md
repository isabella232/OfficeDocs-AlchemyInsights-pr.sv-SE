---
title: 646 Så här konfigurerar du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722581"
---
# <a name="configure-sync-features"></a>Konfigurera synkroniseringsfunktioner

Azure AD Connect innehåller flera funktioner som är aktiverade som standard eller som du kan aktivera senare. Vissa funktioner kräver ytterligare konfiguration i specifika miljöer.

- [Filtreringsgränser](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekten synkroniseras till Azure AD. Som standard synkroniseras alla användare, kontakter, grupper och Windows 10-datorkonton. Du kan inkludera eller utesluta objekt baserat på domäner, ru:er eller andra attribut.

- [Synkronisering av lösenord hash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösenordshhen från den lokala Active Directory till Azure AD. Detta möjliggör lösenordshantering på en plats, men användning av samma lösenord i både lokala miljöer och molnmiljöer. Eftersom Active Directory är den auktoritära källan kan du använda dina egna lösenordsprinciper.

- [Med självbetjäningslösenordsåterställning (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösenord i molnet samtidigt som de tillämpar din lokala lösenordsprincip.

- [Enhetsåterskrivning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gör att registrerade enheter i Azure AD kan skrivas tillbaka till den lokala Active Directory så att de kan användas för villkorlig åtkomst.

- [Förhindra oavsiktliga borttagningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverat som standard för att förhindra för många samtidiga objektborttagningar (fler än 500 objekt per synkronisering). Du kan ändra den här inställningen så att den uppfyller organisationens behov.

- [Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverad som standard för expressinstallationer och säkerställer att din version av Azure AD Connect alltid är aktuell.
