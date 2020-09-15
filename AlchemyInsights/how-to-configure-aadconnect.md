---
title: 646 så här konfigurerar du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704507"
---
# <a name="configure-sync-features"></a>Konfigurera synkroniseringsfunktionen

Azure AD Connect innehåller flera funktioner som är aktiverade som standard eller som du kan aktivera senare. För vissa funktioner krävs ytterligare konfiguration i specifika miljöer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begränsar objekten synkroniseras till Azure AD. Som standard synkroniseras alla användare, kontakter, grupper och Windows 10-dator konton. Du kan ta med eller utesluta objekt baserat på domäner, organisationsenheter eller andra attribut.

- [Lösenordsskyddade lösen ord](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserar lösen ords-hashvärdet från den lokala Active Directory till Azure AD. Detta tillåter lösen ords hantering på en och samma plats men använder samma lösen ord i både lokala och moln miljöer. Eftersom Active Directory är en auktoritativ källa kan du använda dina egna lösen ords principer.

- Med [självbetjäning för återställning av lösen ord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) kan användare återställa sina egna lösen ord i molnet och ändå tillämpa din lokala lösen ords princip.

- Med funktionen för att [Ångra](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) kan registrerade enheter i Azure AD skrivas tillbaka till den lokala Active Directory så att de är avsedda för villkorlig åtkomst.

- [Förhindra att oavsiktlig borttagning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverat som standard för att förhindra alltför många objekt borttagningar samtidigt (fler än 500 objekt per synkronisering). Du kan ändra den här inställningen för att uppfylla organisationens behov.

- [Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är aktiverat som standard för Express installationer och säkerställer att din version av Azure AD Connect alltid är aktuell.
