---
title: 932 uppgradera AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389777"
---
# <a name="upgrade-azure-ad-connect"></a>Uppgradering av Azure AD Anslut

Som standard aktiveras automatisk uppgradering för Azure AD Connect, som hjälper till att se till att du kör den senaste versionen. Om du vill kontrollera inställningarna för automatisk uppgradering använder du cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet returnerar ett av följande värden: 

- **Aktiverad**: automatisk uppgradering är aktiverad.

- **Inaktiverad**: automatisk uppgradering har inaktiverats.

- **Suspended**: systemet inte längre är berättigad till automatiska uppgraderingar. Du kan inte konfigurera den här värde. den anges av systemet. 

Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Om du vill hämta den senaste versionen av Azure AD Connect, gå till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
