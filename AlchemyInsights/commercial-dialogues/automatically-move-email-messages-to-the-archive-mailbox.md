---
title: Automatiskt flytta e-postmeddelanden till arkivpostlådan
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749290"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatiskt flytta e-postmeddelanden till arkivpostlådan

Så här skapar du en princip för att automatiskt flytta en användares gamla e-post till arkivpostlådan:

1. Gå till [**Säkerhet & för**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **efterlevnadsdatastyrning**  >  **för** att verifiera att en arkivpostlåda har aktiverats för användaren. Om det inte har gjort det klickar **du på** Aktivera **och sedan** Ja i varningsrutan.
2. Gå till [**Exchange admin center > för efterlevnadshantering > bevarandetaggar**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Välj ikonen + och välj sedan **automatiskt tillämpas på hela postlådan.**
4. Tilldela bevarandetaggen ett namn och välj **Flytta till arkiv.** Ange hur lång tid du vill ha kvarhållningstiden, till exempel 90 dagar. Klicka på **Spara**.
5. Skapa nu en bevarandeprincip: välj **bevarandeprinciper** och välj ikonen för att lägga till en ny princip.
6. Ge bevarandeprincipen ett namn och klicka sedan på och bläddra för att hitta och lägga till den bevarandetagg du just skapade. Klicka på **Spara**.
7. Tillämpa slutligen kvarhållningsprincipen på användarens postlåda: gå till mottagarnas postlådor i administrationscentret  >  **för** Exchange. Välj alla användare som du vill tillämpa principen på och välj sedan **Redigera** (pennikonen).
8. Klicka på postlådefunktioner **i dialogrutan.** Tillämpa **den princip** som du just skapade när du > Spara under **Bevarandeprincip.**
9. Instruktioner för hur du tillämpar principen på alla användare finns i [Använda en bevarandeprincip för postlådor.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
