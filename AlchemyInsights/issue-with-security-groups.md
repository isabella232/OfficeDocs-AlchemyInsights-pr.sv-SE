---
title: Problem med säkerhetsgrupper
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177634"
---
# <a name="issue-with-security-groups"></a>Problem med säkerhetsgrupper

**Om du får nätverksfel AADDS104**

Ogiltiga nätverkssäkerhetsgruppsregler är den vanligaste orsaken till nätverksfel för Azure Active Directory DS (AD DS). Nätverkssäkerhetsgruppen för det virtuella nätverket måste tillåta åtkomst till specifika portar och protokoll. Om dessa portar är blockerade kan Azure-plattformen inte övervaka eller uppdatera den hanterade domänen. Synkroniseringen mellan Azure AD och Azure AD DS påverkas också. Se till att ha standardportarna öppna för att undvika avbrott i tjänsten.

Information om hur du förstår och löser vanliga varningar för konfigurationsproblem för säkerhetsgrupper i nätverket finns i [Lägga till och verifiera säkerhetsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
