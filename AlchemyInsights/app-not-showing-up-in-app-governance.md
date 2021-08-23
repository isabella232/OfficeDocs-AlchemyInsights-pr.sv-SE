---
title: Mitt program visas inte i Appstyrning
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454989"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Mitt program visas inte i Appstyrning

Om programmet inte visas i appstyrning ska du kontrollera följande:

1. Gå till [Azure AD och](https://aad.portal.azure.com/) leta reda på programmets program-ID genom att söka efter appnamnet i det översta fältet på sidan Översikt.

1. Få Graph i Utforskaren och sök efter app-ID i tjänstens huvudnamn genom att använda den här frågan och ersätta med relevant <appId> program-ID: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Om inga resultat returneras söker du efter program-ID:t i programmet genom att använda den här frågan och ersätta med <appId> relevant program-ID: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Om du har problem med frågan kan du läsa [Få support.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Mer information eller insikter om dina appar i appstyrning finns i [Läs mer om synlighet och insikter.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Mer information om hur du visar appar finns i [Visa dina appar](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
