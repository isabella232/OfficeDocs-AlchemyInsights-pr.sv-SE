---
title: Felsöka felkoder för Azure AD-autentisering och auktorisering (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037840"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Felsöka felkoder för Azure AD-autentisering och auktorisering (AADSTS)

Så här löser du AAD-autentiserings- och auktoriseringsfelkoder (AADSTS):

1. **Hantera felkoder i programmet**

- **OAuth2.0-specifikationer**, innehåller anvisningar om hur fel hanteras under autentisering med hjälp av https://tools.ietf.org/html/rfc6749#section-5.2 feldelen av felsvaret.

    - **fel**: En felkodssträng som kan användas för att klassificera typer av fel som uppstår och ska användas för att reagera på fel.
    - **Felfältet** har flera möjliga värden – granska protokolldokumentationslänkarna och OAuth 2.0-specifikationerna för mer information om specifika fel och hur du reagerar på dem.

- Här är ett exempel på ett felsvar:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Slå upp aktuell information om felkoden**

- Felkoder och felmeddelanden kan komma att ändras. Den senaste informationen finns på sidan för att hitta beskrivningar av https://login.microsoftonline.com/error AADSTS-fel, korrigeringar och några förslag på lösningar.
- Du kan också söka efter och felsöka [AADSTS-felkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) som listas i artikeln [Azure AD-autentiserings- och auktoriseringsfelkoder.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Få hjälp**

- [Support- och hjälpalternativ](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) för utvecklare – Om du behöver ett svar på en fråga eller hjälp med att lösa ett problem som inte finns i vår dokumentation kan det vara dags att kontakta experter för att få hjälp. I den här artikeln får du flera förslag på hur du får svar på dina frågor när du utvecklar appar som integreras med Microsofts identitetsplattform.








