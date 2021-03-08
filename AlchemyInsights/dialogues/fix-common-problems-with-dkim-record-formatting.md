---
title: Åtgärda vanliga problem med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525644"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Åtgärda vanliga problem med DKIM-postformatering

De flesta problem med DKIM-konfiguration är relaterade till felaktiga DNS-poster.

Åtgärda problem med DKIM-uppsättningen genom att kontrollera att DKIM CNAME-posten **(inte** en TXT-post) är rätt formaterad. Mer information finns i Vad [du behöver göra för att konfigurera DKIM manuellt i Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Om du behöver hjälp med DNS-poster i allmänhet kan du gå till Skapa DNS-poster hos valfri [DNS-värd för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> När du har skapat eller uppdaterat DKIM DNS-posterna på DNS-värdtjänsten för din domän måste du vänta tills DNS-posterna har spridits.
