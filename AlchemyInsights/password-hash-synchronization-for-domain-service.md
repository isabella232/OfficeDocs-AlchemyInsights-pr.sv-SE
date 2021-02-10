---
title: Synkronisering av lösenordshashar för domäntjänst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177620"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synkronisering av lösenordshashar för domäntjänst

**Om din Azure AD DS-instans uppmanar dig att aktivera synkronisering av lösenordshashar**

Du stöter på ett scenario där du kör en hybridmiljö med användare som synkroniserar från en lokal Azure Active Directory DS-miljö (AD DS). Det här scenariot påträffas trots att du har synkronisering av lösenordshashar från den lokala AD DS till Azure AD-klienten.

**Orsak**

Det här händer eftersom Azure AD Connect som standard inte synkroniserar äldre NTLM-lösenordshanterare (New Technology LAN Manager) och Kerberos-lösenordshashar som krävs för Azure AD DS.

**Lösning** 

Du måste konfigurera Azure AD Connect för att synkronisera de lösenordshashar som krävs för NTLM- och Kerberos-autentisering.

När Azure AD Connect har konfigurerats synkroniseras sedan även äldre lösenordshashar till Azure AD vid skapande av lokalt konto eller ändring av lösenord. Mer information [om](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) detta och anvisningar om hur du aktiverar lösenordssynkronisering i Azure AD DS hybridmiljöer finns här.