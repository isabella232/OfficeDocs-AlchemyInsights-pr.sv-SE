---
title: Konfigurera domän tjänst
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885686"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Det går inte att aktivera AAD-DS eller distributionen fungerar inte

Utför följande steg för att lösa problemet med att Azure AD Domain Service (AAD-DS) inte aktive ras eller att det inte går att distribueras:

1. Om du använder ett befintligt virtuellt nätverk kontrollerar du dina NSG för regler som blockerar de portar som behövs för att synkroniseras i AAD-DS i portalen https://aka.ms/aadds-networking .
2. Kontrol lera om fel meddelandet besvaras i den här fel söknings guiden som är tillgänglig i  https://aka.ms/aadds-troubleshoot-enable .
3. Försök Distribuera Azure AD Domain Services i ett nytt virtuellt nätverk.
4. Följ start guiden för hur du distribuerar AAD-DS: [skapa och konfigurera AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Om du har problem med distributionen av Azure AD Domain Services läser du [Felsöka Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) för att lösa vanliga fel för att få saker att fungera igen. 

**Det går inte att inaktivera AAD-DS**

AAD – kunde inte pausas. Om du vill sluta använda den hanterade domänen måste den tas bort.
Information om hur du tar bort en hanterad domän finns i [ta bort AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



