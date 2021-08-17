---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312705"
---
# <a name="alert-policies"></a>Aviseringsprinciper

Microsoft 365 innehåller [standardprinciper](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) för aviseringar som utlöser aviseringar för organisationer med en Microsoft 365 Enterprise- eller Microsoft 365 för myndigheter i USA, abonnemang E1/G1, E3/G3 eller E5/G5. Därför kan administratörer få ett e-postmeddelande med avisering som skickas från Office365Alerts@microsoft.com med en ämnesrad, till exempel "En avisering med låg allvarlighetsgrad: namn på *aviseringsprincip".* Aviseringsaviseringar skickas när aviseringar utlöses för vanliga aktiviteter, till exempel när användare:

- Skapa inkorgsregler som vidarebefordrar e-post.
- Tilldela behörigheter till postlådan.
- Dela eller ta bort ett stort antal filer i SharePoint och fildelning.
- Skapa eDiscovery-sökningar och exportera sökresultat.

Granska och agera på en avisering:

1. Gör något av följande:
   - I Microsoft 365 Efterlevnadscenter på <https://compliance.microsoft.com> går du till **Aviseringar**. Du kan också använda om du vill gå **direkt** till sidan <https://compliance.microsoft.com/compliancealerts> Aviseringar.
   - Gå till Microsoft 365 Defender alla aviseringar <https://security.microsoft.com> i & i **portalen** \> **.** Du kan också använda om du vill gå **direkt** till sidan <https://security.microsoft.com/alerts> Aviseringar.
2. Klicka på en avisering om du vill visa en utfällsida med information om aviseringen.

Du kan vidta åtgärder för en avisering, t.ex. [ta bort en regel för misstänkt inkorg.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Du kan också stänga aviseringen genom att klicka **på Lös på** den utfällade aviseringssidan.

Mer information om hur du konfigurerar och hanterar aviseringsprinciper finns i [den här artikeln.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Viktigt:** Avisering om e-postaviseringar från Microsoft ber dig aldrig att göra följande:

- Ange ett lösenord
- Kontrollera säkerhetsinformationen för ditt konto
- Autentisera dig igen

Om du får ett e-postmeddelande med den här typen av förfrågningar har det inte skickats av Microsoft och bör ses som nätfiske. Om du får ett meddelande med den här typen av förfrågningar [ska du rapportera meddelandet till Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
