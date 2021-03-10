---
title: Exempel på en policy för nätfiske i Microsoft Defender för Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695640"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exempel på en policy för nätfiske i Microsoft Defender för Office 365

Dessa inställningar aktiverar en princip som heter *Domän och VD.* Med den här principen skyddas både användare och domäner från personifiering och sedan tillämpas principen på all e-post som tas emot av användare inom domänen. Lägg först till följande information för att skapa principen:

- **Namn:** Domän och VD **Beskrivning:** Säkerställer att VD och din domän inte utger sig för att vara imiterade.
  **Används för:** Välj **mottagarens domän är.** Under **Valfri av dessa** väljer **du** Välj och sedan en domän. Välj **+ Lägg till.** Markera kryssrutan bredvid namnet på domänen i listan (till exempel *contoso.com)* och välj sedan **Lägg till.** Välj **Klar**.
- När principen har skapats kan du finjustera principen med hjälp av följande alternativ:
  - **Lägg till användare som ska skydda:** I det här exemplet ska du åtminstone lägga till VD:s e-postadress.
  - **Lägg till domäner som ska** skyddas: Lägg till den organisationsdomän som innehåller VD-kontoret.
  - **Välj åtgärder:** Om e-post skickas av en imiterad användare väljer du Omdirigera meddelandet till en annan e-postadress och anger sedan säkerhetsadministratörens e-postadress (till *exempel securityadmin@contoso.com).*  Om **e-post skickas med en imiterad domän** väljer du **Sätt meddelandet i karantän.**
  - **Postlådeinformation:** Det här alternativet väljs som standard när du skapar en ny princip mot nätfiske. Låt inställningen vara **på för** bästa resultat.
  - **Lägg till betrodda avsändare och domäner:** I det här exemplet ska du inte definiera några åsidosättningar.
- När du har granskat inställningarna väljer du Skapa den **här principen** eller **Spara** efter behov.

Mer information finns i Principer [för skydd mot nätfiske i Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
