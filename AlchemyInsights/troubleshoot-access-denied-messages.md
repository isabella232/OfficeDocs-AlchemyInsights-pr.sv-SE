---
title: Felsöka meddelanden om nekad åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939901"
---
# <a name="troubleshoot-access-denied-messages"></a>Felsöka meddelanden om nekad åtkomst

Om någon fick meddelandet "Åtkomst nekad" till en delad mapp i SharePoint kan webbplatssamlingsadministratören ha aktiverat nedlåst behörighetsläge för användare med begränsad åtkomst. Så här inaktiverar du den här frågan: 
  
1. Bläddra till webbplatsen, klicka på ikonen Inställningar och klicka sedan på **Webbplats Inställningar**.
    
2. Klicka **på Webbplatssamlingens** funktioner **under Administration av webbplatssamling.**
    
3. Klicka **på Inaktivera bredvid Nedlåst behörighetsläge för användare** med begränsad **åtkomst.**
    
Ett meddelande om nekad åtkomst kan också ske för delade mappar om webbplatsen är en publiceringswebbplats. Mer information finns i [Åtkomst nekas vid åtkomst till en delad mapp.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Om någon fick meddelandet "Åtkomst nekad" när han eller hon försöker visa åtkomstförfrågningar måste användaren läggas till som antingen webbplatssamlingsadministratör eller medlem i gruppen Ägare för webbplatsen. Mer information finns i listan [Åtkomst nekad till åtkomstbegäranden.](https://go.microsoft.com/fwlink/?linkid=2004220)
  
Om en användare fick meddelandet "Åtkomst nekad" efter att ha tagits bort från active directory lokalt och sedan lagts till igen, se Åtkomst nekad när ett användarkonto synkroniseras till [ett Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

