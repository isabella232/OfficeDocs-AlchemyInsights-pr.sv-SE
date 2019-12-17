---
title: Felsöka åtkomst nekad-meddelanden
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050723"
---
# <a name="troubleshoot-access-denied-messages"></a>Felsöka åtkomst nekad-meddelanden

Om någon har fått meddelandet "åtkomst nekad" till en delad mapp i SharePoint, kan administratören för webbplatssamlingen ha aktiverat läget "begränsad åtkomst till användarbehörighet". Så här stänger du av: 
  
1. Bläddra till webbplatsen, klicka på ikonen Inställningar och klicka sedan på **Webbplatsinställningar**.
    
2. Klicka på **Webbplatssamlingens funktioner**under **Administration av webbplatssamling**.
    
3. Bredvid **begränsad åtkomst användarbehörighet låsning läge**, klickar du på **inaktivera**.
    
Ett meddelande om nekad åtkomst kan också uppstå för delade mappar om webbplatsen är en publiceringswebbplats. Mer information finns i [åtkomst nekad vid åtkomst till en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Om en person har fått meddelandet "åtkomst nekad" när du försöker visa åtkomstbegäranden måste användaren läggas till som en webbplatssamlingsadministratör eller medlem i gruppen ägare för webbplatsen. Mer information finns i [åtkomst nekad till listan åtkomstbegäranden](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Om en användare har fått meddelandet "åtkomst nekad" efter att de har tagits bort från Active Directory lokalt och sedan lagts till igen, se [åtkomst nekad när ett användarkonto har synkroniserats till Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

