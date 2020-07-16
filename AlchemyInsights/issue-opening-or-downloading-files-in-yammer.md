---
title: Problem med att öppna eller ladda ned filer i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148437"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem med att öppna eller ladda ned filer i Yammer

Classic Yammer stöder flera alternativ för filuppladdningar till meddelanden och grupper. Beroende på nätverkskonfiguration, filer som standard lagring i SharePoint.

Filväljaren i nya Yammer stöder ännu inte alla alternativ som finns i klassiska Yammer. En framtida uppdatering kommer att lägga till ytterligare funktioner. Mer information finns i [Bifoga en fil eller bild i ett Yammer-konversationsinlägg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Det går inte att öppna eller hämta en fil**  

En fil kan överföras till Yammer men också länka till en fil i SharePoint Online. Om du vill felsöka måste du först bestämma platsen för filen. Om filen har överförts till Yammer har den en *.yammer.com-URL. Kontrollera att nödvändiga webbadresser och IP-adresser är avblockerade. Mer information finns i blogginlägget [Använda hårdkodade IP-adresser för Yammer rekommenderas inte](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Kontrollera om en användare som också är global administratör kan hämta filen. Om filen är privat kan du behöva använda privat innehållsläge. Mer information finns [i Övervaka privat innehåll i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gäster och filer på Yammer-nätverksnivå i SharePoint Online**  

[Gäster på nätverksnivå i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) använder inte Azure AD B2B och är interna för Yammer-tjänsten, så att de inte kan komma åt Yammer-filer som lagras i SharePoint. Skapa en extern AAD B2B-användare som kan komma åt dokumentbibliotek i SharePoint Online med hjälp av den identiteten. Information om framtida Azure AD B2B-gästsupport i Yammer finns [i B2B-gästsupport (Business-to-business) i Yammer Preview – Kundvillkor och vanliga frågor](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)och svar .