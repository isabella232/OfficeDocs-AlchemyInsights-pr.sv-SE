---
title: Blockera användarbaserade e-postsignaturer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243636"
---
# <a name="block-user-made-email-signatures"></a>Blockera användarbaserade e-postsignaturer

Följande lösning gäller endast för e-postsignaturer som skapas i Outlook på webben. Du kan bara blockera signaturer i Outlook-appen om du har en lokal Exchange Server.

1. Välj Administrationscenter för Exchange i  >  **administrationscentret.**
2. Klicka **på behörigheter** för Outlook Web  >  **App-principer.**
3. Markera principen och klicka sedan på pennikonen för att redigera den.
4. Klicka **på fler** alternativ för  >  **funktioner.**
5. Avmarkera kryssrutan E-postsignatur **under** Användarupplevelse och klicka sedan på **Spara.** 

**Viktigt:** Om en signatur har lagts till innan du avmarkerar den här kryssrutan kan användaren fortfarande använda den. Be dem att ta bort den.
