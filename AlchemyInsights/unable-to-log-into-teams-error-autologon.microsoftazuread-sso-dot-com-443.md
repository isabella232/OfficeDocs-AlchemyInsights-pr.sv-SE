---
title: Det går inte att logga in på Teams på grund av fel autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038418"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Det går inte att logga in på Teams på grund av fel autologon.microsoftazuread-sso dot com:443

Om sömlös SSO är aktiverad som O365-autentisering kan URL-adressen "autologon.microsoftazuread-sso.com" behöva läggas till i intranätplatser.  Om den redan har lagts till på betrodda platser och sömlös SSO används ska den tas bort från betrodda platser.

Läs [Checklista för felsökning i sömlös SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Följ dessa steg om du vill lägga till en URL-adress i listan över intranät-webbplatser:

1. Öppna Internet Explorer genom att klicka på knappen **Start**. I sökrutan skriver du Internet Explorer och klickar sedan på **Internet Explorer** i resultatlistan.
2. Klicka på **Verktyg** och klicka sedan på **Internetalternativ**.
3. Klicka på fliken **Säkerhet**.
4. Klicka nu på **Lokala intranät-webbplatser** och klicka sedan på knappen **Webbplatser** och sedan knappen **Avancerat**.
5. Ange webbplatsens URL och klicka på **Lägg till**.
6. Klicka på **Stäng** när du är klar.

Mer information finns i [Dokumentation för distribution av sömlös SSO för O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inkluderar principbaserad process för att lägga till en URL-adress till intranät-webbplatser i steg 3).
