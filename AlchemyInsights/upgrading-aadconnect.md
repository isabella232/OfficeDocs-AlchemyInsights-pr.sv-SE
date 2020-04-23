---
title: 932 Uppgradering av AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766511"
---
# <a name="upgrade-azure-ad-connect"></a>Uppgradera Azure AD Connect

Som standard är automatisk uppgradering aktiverad för Azure AD Connect, vilket hjälper till att säkerställa att du kör den senaste versionen. Om du vill verifiera de automatiska uppgraderingsinställningarna använder du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten returnerar ett av följande värden:

- **Aktiverad**: Automatisk uppgradering är aktiverad.

- **Inaktiverad**: Automatisk uppgradering är inaktiverad.

- **Pausad**: Systemet är inte längre berättigat till automatiska uppgraderingar. Du kan inte konfigurera det här värdet. den är inställd av systemet.

Mer information finns i [Automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Om du vill hämta den senaste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)versionen av Azure AD Connect går du till .
