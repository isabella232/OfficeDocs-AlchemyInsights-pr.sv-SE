---
title: Vill du rapportera skräppost felaktigt till Microsoft?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396633"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Markeras riktiga meddelanden som skräppost?

Det är frustrerande när ett legitimt e-postmeddelande hamnar i skräppostmappen eller i karantän. Tänk på de här vanligaste orsakerna till falska positiva resultat:

**Åsidosättningar av klientorganisation (vanligaste)** Detta är helt inom din kontroll för att åtgärda.

Skicka meddelandet på Microsoft 365 Defender för analys av de effektande principerna och reglerna. Mer information finns tillgänglig inom några minuter.
Granska eller ändra principer eller regler efter vad som är tillämpligt. 

**Åsidosättningar för slutanvändare (vanligt)** Detta är helt inom din kontroll för att åtgärda. 

Skicka meddelandet på Microsoft 365 Defender för analys av de effektande principerna och reglerna. Mer information finns tillgänglig inom några minuter. 

Om ett meddelande har blockerats på grund av att det skickades från en adress i en användares lista med spärrade avsändare innehåller rubrikerna filtreringsaviseringar av skräppost "SFV:BLK".

**Avsändarnas e-postautentisering** Detta är delvis inom din kontroll för att åtgärda.

Skicka meddelandet för att analysera fel i avsändarens e-postautentisering vid leverans. resultaten är tillgängliga inom en dag. 

Om du äger den avsändande infrastrukturen bör du granska hur du justerar den med SPF, DKIM och DMARC för att se till att mål-e-postsystem litar på meddelanden som skickas från din domän. Du kan också kontakta avsändarna för att lösa DNS-konfigurationerna.

**Microsoft-filtrerings filtrerande beslut** Detta är delvis inom din kontroll för att åtgärda.

Skicka meddelandet och rapportera meddelandet som säkert. sökning efter resultat är tillgänglig inom en dag. Använd klientorganisationens lista över tillåtna/blockerade, om du inte är nöjd med filtrering av bedömningar i vissa situationer. Men du bör inte permanent kringgå Microsoft-filtrerings filtrerande beslut. 

Mer information finns i:

- Gör det möjligt för slutanvändarna att skicka meddelanden till Microsoft. Microsoft använder dessa inskickade e-postskyddstekniker för att göra dem mer effektiva, och de visas i inskickade rapporter som en indikation på hur principer ska uppdateras. 

- En kort video om hur du skickar meddelanden för analys finns i [Skicka meddelanden för analys](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Använd administrationsinskick för att skicka misstänkt skräppost, nättr ut, URL:er och filer till Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Hantera Klientorganisationens Tillåt/blockera-listan](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Meddelandehuvuden för antiskräppost i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Skydd mot utgående skräppost i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)