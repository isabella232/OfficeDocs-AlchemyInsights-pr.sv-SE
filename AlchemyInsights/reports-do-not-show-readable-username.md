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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327832"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapporter i Administrationscenter för Microsoft 365 visar inte läsbart användarnamn

I Administrationscenter för Microsoft 365 visas inte användarnamn, utan visar i stället alfanumeriska värden som B2BC6C15BB9FCDEA71E5CD302D228CC8.

Detta är normalt och har meddelats i Meddelandecenter (MC275344, publicerad 3 augusti 2021). 

Globala administratörer kan återställa den här ändringen för sin klientorganisation och visa identifierbar användarinformation om organisationens sekretesspolicy tillåter det. Så här återställer du ändringen för klientorganisationen:

1. I administrationscentret går du **Inställningar**  >  **Organisationsinställningar** >  [**Tjänster**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) och väljer **Rapporter**. 
1. Under **Välj hur användarinformation ska visas** väljer du **Visa identifierbar användarinformation i rapporter** och kör sedan rapporten igen.