---
title: Åtgärda vanliga problem med Microsoft Defender för Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330078"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Åtgärda vanliga problem med Microsoft Defender för Office 365

Här är några lösningar på vanliga problem med Microsoft Defender för Office 365:

- **Meddelandefördröjning:**

  Fördröjningar i e-postleveransen kan Valv av meddelanden. Mer information finns i Valv [principinställningar för bifogade filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Rapportera falska positiva eller negativa resultat:**

  Mer informations finns i [Anmäla meddelanden och filer till Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Aktivera Valv länkskydd:**

  1. I portalen Microsoft 365 Defender på går du till E-& för samarbete & principer för hot <https://security.microsoft.com/>  \>  \>  \> **Valv i** **avsnittet** Principer.

     Om du vill gå **direkt Valv sidan** Länkar använder du <https://security.microsoft.com/safelinksv2> .

  2. På **Valv Länkar** markerar du principen genom att klicka på namnet på principen.
  3. Gör något av följande i den utfällade informationen som visas:
     - Om du vill lägga till en ny princip väljer **du + Skapa.** En guide startas så att du kan definiera dina principinställningar.
     - Om du vill redigera en befintlig princip markerar du principen genom att klicka på namnet på principen. I den utfäll syns informationen väljer du **Redigera** i **avsnittet Skyddsinställningar.**
  4. Konfigurera **följande inställningar** på sidan Skyddsinställningar:
     - Aktivera Välj **åtgärden för okända potentiellt skadliga URL-adresser i meddelanden.**
     - Välj **Använd säkra länkar för meddelanden som skickas inom organisationen.**

  Mer information finns i Konfigurera [principer Valv länkar i Microsoft Defender för Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
