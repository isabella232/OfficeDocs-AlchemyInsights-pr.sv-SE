---
title: 932 uppgraderar AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806057"
---
# <a name="upgrade-azure-ad-connect"></a>Uppgradera Azure AD Connect

Automatisk uppgradering är aktive rad som standard för Azure AD Connect, vilket säkerställer att du kör den senaste versionen. Om du vill kontrol lera inställningarna för automatisk uppgradering använder du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten returnerar ett av följande värden:

- **Enabled**: automatisk uppgradering är aktiverat.

- **Disabled**: automatisk uppgradering är inaktiverat.

- **Upphävda**: systemet är inte längre berättigat att få automatiska uppgraderingar. Det går inte att konfigurera det här värdet; Det är inställt av systemet.

Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Om du vill ladda ned den senaste versionen av Azure AD Connect går du till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
