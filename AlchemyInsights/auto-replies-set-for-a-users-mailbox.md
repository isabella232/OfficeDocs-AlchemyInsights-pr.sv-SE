---
title: Konfigurera automatiska svar för en postlåda
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788900"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Konfigurera automatiska svar för en användares postlåda

**Metod 1**

1. Logga in på Microsoft 365-portalen.

2. Gå till **Användare > Aktiva användare** (eller **Grupper > Delade postlådor** om du konfigurerar detta på en delad postlåda).

3. Välj en användare som har en Microsoft Exchange-postlåda.

4. I den utfällbara menyn till höger går du till **E-postinställningar > Automatiska svar** (om det är en delad postlåda klickar du på **Automatiska svar** i den utfällbara menyn).

**Metod 2**

1. Logga in på administrationsportalen för Microsoft 365 med administratörens autentiseringsuppgifter.

2. Expandera **Administrationscenter** och klicka sedan på **Exchange**.

3. Klicka på bilden i det övre högra hörnet, klicka på **En annan användare** och välj sedan den användarpostlåda som du vill ändra.

4. På vänster sida väljer du **Alternativ**, klickar på **Ordna e-post** och sedan på **Automatiska svar.**

**Metod 3**

Kör följande cmdlet i Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Mer information om den här cmdleten finns i [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
