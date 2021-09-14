---
title: Rapporter i Administrationscenter för Microsoft 365 visar inte läsbart användarnamn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316353"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapporter i Administrationscenter för Microsoft 365 visar inte läsbart användarnamn

I Administrationscenter för Microsoft 365 visas inte användarnamn, utan visar i stället alfanumeriska värden som B2BC6C15BB9FCDEA71E5CD302D228CC8.

Detta är normalt och har meddelats i Meddelandecenter (MC275344, publicerad 3 augusti 2021). 

Globala administratörer kan återställa den här ändringen för sin klientorganisation och visa identifierbar användarinformation om deras organisations sekretessrutiner tillåter. Så här återställer du ändringen för klientorganisationen:

1. I administrationscentret går du **Inställningar**  >  **Inställningar för**  >  [**Org**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)och väljer **Rapporter**. 
1. Under **Välj hur användarinformation ska visas** väljer du Visa identifierbar **användarinformation i** rapporter och kör sedan rapporten igen.