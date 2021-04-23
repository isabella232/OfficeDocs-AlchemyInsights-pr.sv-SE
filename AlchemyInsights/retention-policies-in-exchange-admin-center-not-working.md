---
title: Bevarandeprinciper i administrationscentret för Exchange fungerar inte
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952246"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Bevarandeprinciper i administrationscentret för Exchange

Om du vill att vi ska köra automatiska kontroller för inställningarna som nämns nedan väljer du bakåtknappen < – högst upp på den här sidan och anger sedan e-postadressen till den användare som har problem med bevarandeprinciper.

Om du har problem med bevarandeprinciper i administrationscentret för Exchange som inte gäller för postlådor eller objekt som inte flyttas till arkivpostlådan kontrollerar du följande:

**Rotorsaker:**

- **Assistenten för hanterade** mappar har inte bearbetat användarens postlåda. Assistenten för hanterade mappar försöker att bearbeta alla postlådor i den molnbaserade organisationen en gång var sju:e dag.

  **Lösning:** Kör assistenten för hanterade mappar.

- **RetentionHold** har **aktiverats** för postlådan. Om postlådan har placerats på ett RetentionHold bearbetas inte bevarandeprincipen för postlådan under den tiden.

  **Lösning:** Kontrollera status för inställningen Bevarande av bevarande och uppdatera efter behov. Mer information finns i [Bevarande av postlåda.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Obs!** Om en postlåda är mindre än 10 MB bearbetar inte assistenten för hanterade mappar automatiskt postlådan.
 
Mer information om bevarandeprinciper i administrationscentret för Exchange finns i:

- [Bevarandetaggar och bevarandeprinciper](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Använda en bevarandeprincip på postlådor eller Lägga](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [till eller ta bort bevarandetaggar](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Identifiera typen av undantag som tillämpas på en postlåda](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
