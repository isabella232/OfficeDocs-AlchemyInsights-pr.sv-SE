---
title: Exempel på en Microsoft Defender Office 365 nätfiskeprincip
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035024"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exempel på en Microsoft Defender Office 365 nätfiskeprincip

De här inställningarna aktiverar en princip som *heter Domän och VD.* Med den här principen skyddas både användare och domäner från personifiering och sedan tillämpas principen på all e-post som tas emot av användare i domänen. Lägg först till följande information för att skapa principen:

- **Namn**: Beskrivning av domän **och** VD : Säkerställer att VD och din domän inte utger sig för att vara.
  **Används för:** Välj **Mottagarens domän är**. Under **Valfri av dessa** väljer du **Välj** och sedan en domän. Välj **+ Lägg till.** Markera kryssrutan bredvid namnet på domänen i listan (till exempel klicka på *contoso.com*) och välj sedan Lägg **till**. Välj **Klar**.
- När principen har skapats kan du finjustera principen med hjälp av följande alternativ:
  - **Lägga till användare att skydda:** I det här exemplet ska du som minst lägga till VD:s e-postadress.
  - **Lägg till domäner att** skydda: Lägg till organisationsdomänen som innehåller vd:s kontor.
  - **Välj åtgärder:** För **Om** e-post skickas av en imiterad användare väljer du Omdirigera meddelandet till en annan e-postadress och anger sedan e-postadressen till säkerhetsadministratören (till *exempel securityadmin@contoso.com*). För **Om e-post skickas med en imiterad domän** väljer du Sätt meddelandet i **karantän.**
  - **Postlådeinformation:** Det här alternativet är valt som standard när du skapar en ny princip mot nätfiske. Lämna den här inställningen **På** för bästa resultat.
  - **Lägga till betrodda avsändare och domäner:** I det här exemplet ska du inte definiera några åsidosättningar.
- När du har granskat inställningarna väljer du Skapa **den här principen** eller **Spara** efter behov.

Mer information finns i [Principer för skydd mot nätfiske i Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
