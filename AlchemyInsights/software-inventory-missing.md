---
title: Programvaruinventering saknas eller är felaktig
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676516"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Programvaruinventering saknas eller är felaktig

Software Inventory in Hantering av hot och säkerhetsrisker (TVM) är en lista över kända program i din organisation med officiella gemensam plattform uppräkning (CPE).

Eventuella svagheter publiceras inte för programvaruprodukter utan ett officiellt CPE. Inventeringen omfattar även information som namnet på leverantören, antal svagheter, hot och antal exponerade enheter.

Programvaruändringar på enheter återspeglas vanligtvis i säkerhetsportaler inom två timmar. Ibland kan det dock ta längre tid. Det finns för närvarande inget sätt att tvinga fram synkronisering. det här är en kontinuerlig bedömning.

Om du har gjort en ändring av programvaran och ändringen inte återspeglas korrekt i TVM efter 5 timmar gör du så här:

1. Kontrollera avsnittet med programvarubevis för att förstå hur programvaran identifierades.
1. Kontrollera att programvaran stöds. Programvaran kan bara visas på enhetsnivå även om den för närvarande inte stöds av Hantering av hot och säkerhetsrisker. Men endast begränsade data finns tillgängliga.
1. Information om hur du rapporterar felaktigheter från portalen finns i [Rapportens felaktigheter.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Obs!** Att rapportera fel från MDE-portalen är en envägskanal för teknik. Om problemet är brådskande ska du öppna ett support ärende.

Mer information finns i Lager [av programvara - Hantering av hot och säkerhetsrisker](/microsoft-365/security/defender-endpoint/tvm-software-inventory).