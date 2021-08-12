---
title: 646 Konfigurera AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963661"
---
# <a name="configure-sync-features"></a>Konfigurera synkroniseringsfunktioner

Azure AD Anslut innehåller flera funktioner som är aktiverade som standard, eller som du kan aktivera senare. Vissa funktioner kräver ytterligare konfiguration i vissa miljöer.

- [Filtreringsbegränsningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) som objekten synkroniseras till Azure AD. Som standard synkroniseras alla användare, kontakter, Windows 10 och alla datorkonton. Du kan inkludera eller exkludera objekt baserat på domäner, OUs eller andra attribut.

- [Synkronisering av](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) lösenordshashar synkroniserar lösenordshashar från den lokala Active Directory till Azure AD. Det möjliggör lösenordshantering på en plats, men användning av samma lösenord i både lokala miljöer och molnmiljöer. Eftersom Active Directory är den auktoritativa källan kan du använda dina egna lösenordsprinciper.

- [Med självbetjäning för återställning](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) av lösenord (SSPR) kan användare återställa sina egna lösenord i molnet samtidigt som de tillämpar din lokala lösenordsprincip.

- [Med tillbakaskrivning](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) av enhet kan registrerade enheter i Azure AD skrivas tillbaka till den lokala Active Directory så att de kan användas för villkorsstyrd åtkomst.

- [Förhindra oavsiktliga borttagningar](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) är aktiverat som standard för att förhindra för många samtidiga objektborttagningar (fler än 500 objekt per synkronisering). Du kan ändra den här inställningen för att uppfylla organisationens behov.

- [Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) är som standard aktiverad för expressinstallationer och ser till att din version av Azure AD Anslut alltid är aktuell.
