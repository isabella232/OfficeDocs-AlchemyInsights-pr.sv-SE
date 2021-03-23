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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="9f4fe-102">Felsöka felkoder för Azure AD-autentisering och auktorisering (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="9f4fe-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="9f4fe-103">Så här löser du AAD-autentiserings- och auktoriseringsfelkoder (AADSTS):</span><span class="sxs-lookup"><span data-stu-id="9f4fe-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="9f4fe-104">**Hantera felkoder i programmet**</span><span class="sxs-lookup"><span data-stu-id="9f4fe-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="9f4fe-105">**OAuth2.0-specifikationer**, innehåller anvisningar om hur fel hanteras under autentisering med hjälp av https://tools.ietf.org/html/rfc6749#section-5.2 feldelen av felsvaret.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="9f4fe-106">**fel**: En felkodssträng som kan användas för att klassificera typer av fel som uppstår och ska användas för att reagera på fel.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="9f4fe-107">**Felfältet** har flera möjliga värden – granska protokolldokumentationslänkarna och OAuth 2.0-specifikationerna för mer information om specifika fel och hur du reagerar på dem.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="9f4fe-108">Här är ett exempel på ett felsvar:</span><span class="sxs-lookup"><span data-stu-id="9f4fe-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="9f4fe-109">**Slå upp aktuell information om felkoden**</span><span class="sxs-lookup"><span data-stu-id="9f4fe-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="9f4fe-110">Felkoder och felmeddelanden kan komma att ändras.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="9f4fe-111">Den senaste informationen finns på sidan för att hitta beskrivningar av https://login.microsoftonline.com/error AADSTS-fel, korrigeringar och några förslag på lösningar.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="9f4fe-112">Du kan också söka efter och felsöka [AADSTS-felkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) som listas i artikeln [Azure AD-autentiserings- och auktoriseringsfelkoder.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)</span><span class="sxs-lookup"><span data-stu-id="9f4fe-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="9f4fe-113">**Få hjälp**</span><span class="sxs-lookup"><span data-stu-id="9f4fe-113">**Get Help**</span></span>

- <span data-ttu-id="9f4fe-114">[Support- och hjälpalternativ](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) för utvecklare – Om du behöver ett svar på en fråga eller hjälp med att lösa ett problem som inte finns i vår dokumentation kan det vara dags att kontakta experter för att få hjälp.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="9f4fe-115">I den här artikeln får du flera förslag på hur du får svar på dina frågor när du utvecklar appar som integreras med Microsofts identitetsplattform.</span><span class="sxs-lookup"><span data-stu-id="9f4fe-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








